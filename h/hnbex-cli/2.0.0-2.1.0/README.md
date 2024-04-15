# Comparing `tmp/hnbex-cli-2.0.0.tar.gz` & `tmp/hnbex_cli-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnbex-cli-2.0.0.tar", last modified: Tue Nov 15 22:06:36 2022, max compression
+gzip compressed data, was "hnbex_cli-2.1.0.tar", last modified: Mon Apr 15 12:11:37 2024, max compression
```

## Comparing `hnbex-cli-2.0.0.tar` & `hnbex_cli-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2022-11-15 22:06:36.173042 hnbex-cli-2.0.0/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35147 2020-08-07 07:14:05.000000 hnbex-cli-2.0.0/LICENSE
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    47389 2022-11-15 22:06:36.173042 hnbex-cli-2.0.0/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6221 2022-11-15 22:03:05.000000 hnbex-cli-2.0.0/README.rst
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2022-11-15 22:06:36.169041 hnbex-cli-2.0.0/hnbex/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2020-08-07 07:14:05.000000 hnbex-cli-2.0.0/hnbex/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       39 2022-11-15 22:03:03.000000 hnbex-cli-2.0.0/hnbex/__main__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1849 2022-11-15 22:03:05.000000 hnbex-cli-2.0.0/hnbex/api.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     5145 2022-11-15 22:03:05.000000 hnbex-cli-2.0.0/hnbex/commands.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     5658 2022-11-15 22:03:05.000000 hnbex-cli-2.0.0/hnbex/console.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1879 2020-08-07 07:14:05.000000 hnbex-cli-2.0.0/hnbex/output.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2022-11-15 22:06:36.169041 hnbex-cli-2.0.0/hnbex/templates/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      238 2022-08-26 06:22:10.000000 hnbex-cli-2.0.0/hnbex/templates/dumb.gnuplot
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      290 2022-08-26 06:22:10.000000 hnbex-cli-2.0.0/hnbex/templates/qt.gnuplot
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2022-11-15 22:06:36.173042 hnbex-cli-2.0.0/hnbex_cli.egg-info/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    47389 2022-11-15 22:06:36.000000 hnbex-cli-2.0.0/hnbex_cli.egg-info/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      357 2022-11-15 22:06:36.000000 hnbex-cli-2.0.0/hnbex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2022-11-15 22:06:36.000000 hnbex-cli-2.0.0/hnbex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       45 2022-11-15 22:06:36.000000 hnbex-cli-2.0.0/hnbex_cli.egg-info/entry_points.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        6 2022-11-15 22:06:36.000000 hnbex-cli-2.0.0/hnbex_cli.egg-info/top_level.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      890 2022-11-15 22:05:39.000000 hnbex-cli-2.0.0/pyproject.toml
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2022-11-15 22:06:36.173042 hnbex-cli-2.0.0/setup.cfg
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-15 12:11:37.865116 hnbex_cli-2.1.0/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35147 2022-07-31 09:51:52.000000 hnbex_cli-2.1.0/LICENSE
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    47483 2024-04-15 12:11:37.865116 hnbex_cli-2.1.0/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6221 2023-01-08 16:58:06.000000 hnbex_cli-2.1.0/README.rst
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-15 12:11:37.863116 hnbex_cli-2.1.0/hnbex/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2022-07-31 09:51:52.000000 hnbex_cli-2.1.0/hnbex/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       39 2022-07-31 10:09:45.000000 hnbex_cli-2.1.0/hnbex/__main__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1980 2024-04-15 11:52:55.000000 hnbex_cli-2.1.0/hnbex/api.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     5402 2024-04-15 12:08:22.000000 hnbex_cli-2.1.0/hnbex/commands.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     5837 2024-04-15 12:07:47.000000 hnbex_cli-2.1.0/hnbex/console.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1855 2024-04-15 11:55:01.000000 hnbex_cli-2.1.0/hnbex/output.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-15 12:11:37.863116 hnbex_cli-2.1.0/hnbex/templates/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      238 2022-07-31 09:51:52.000000 hnbex_cli-2.1.0/hnbex/templates/dumb.gnuplot
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      290 2022-07-31 09:51:52.000000 hnbex_cli-2.1.0/hnbex/templates/qt.gnuplot
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-15 12:11:37.864117 hnbex_cli-2.1.0/hnbex_cli.egg-info/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    47483 2024-04-15 12:11:37.000000 hnbex_cli-2.1.0/hnbex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      389 2024-04-15 12:11:37.000000 hnbex_cli-2.1.0/hnbex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-04-15 12:11:37.000000 hnbex_cli-2.1.0/hnbex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       45 2024-04-15 12:11:37.000000 hnbex_cli-2.1.0/hnbex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       19 2024-04-15 12:11:37.000000 hnbex_cli-2.1.0/hnbex_cli.egg-info/requires.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        6 2024-04-15 12:11:37.000000 hnbex_cli-2.1.0/hnbex_cli.egg-info/top_level.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1045 2024-04-15 12:11:23.000000 hnbex_cli-2.1.0/pyproject.toml
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-04-15 12:11:37.865116 hnbex_cli-2.1.0/setup.cfg
```

### Comparing `hnbex-cli-2.0.0/LICENSE` & `hnbex_cli-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hnbex-cli-2.0.0/PKG-INFO` & `hnbex_cli-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hnbex-cli
-Version: 2.0.0
+Version: 2.1.0
 Summary: CLI tool for displaying exchange rates for Croatian Kuna
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,14 +684,17 @@
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 HNB Exchange Rate CLI
 =====================
 
 Displays exchange rates for Croatian Kuna (HRK) from the Croatian National Bank
 (HNB). Data is fetched from the [HNB API](https://api.hnb.hr/).
```

### Comparing `hnbex-cli-2.0.0/README.rst` & `hnbex_cli-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `hnbex-cli-2.0.0/hnbex/api.py` & `hnbex_cli-2.1.0/hnbex/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# -*- coding: utf-8 -*-
-
 import json
 import logging
 
 from dataclasses import dataclass
 from datetime import date
 from decimal import Decimal
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
 from urllib.error import HTTPError
 from urllib.request import urlopen
 
 logger = logging.getLogger("hnbex")
 
 
 @dataclass(frozen=True)
 class ExchangeRate:
     date: date
     currency_code: str
-    unit_value: int
     buying_rate: Decimal
     median_rate: Decimal
     selling_rate: Decimal
 
 
 class ApiError(Exception):
     pass
 
 
 def fetch_daily(date: date, currency_code: Optional[str] = None) -> List[ExchangeRate]:
-    url = f"https://api.hnb.hr/tecajn/v2?datum-primjene={date}"
+    url = f"https://api.hnb.hr/tecajn-eur/v3?datum-primjene={date}"
 
     if currency_code:
         url += f"&valuta={currency_code}"
 
     return _api_get(url)
 
 
 def fetch_range(currency: str, from_date: date, to_date: date) -> List[ExchangeRate]:
-    url = f"https://api.hnb.hr/tecajn/v2?valuta={currency}&datum-primjene-od={from_date}&datum-primjene-do={to_date}"
+    # Cannot filter by `valuta=USD` or similar because that returns only one day of data, not a range
+    url = f"https://api.hnb.hr/tecajn-eur/v3?datum-primjene-od={from_date}&datum-primjene-do={to_date}"
+    records = _api_get(url)
 
-    return _api_get(url)
+    # So we need to filter manually
+    return [r for r in records if r.currency_code == currency]
 
 
 def _api_get(url: str) -> List[ExchangeRate]:
     logger.debug(">>> GET {}".format(url))
 
     try:
         with urlopen(url) as response:
@@ -55,16 +55,15 @@
         raise ApiError()
 
 
 def _parse_decimal(value: str) -> Decimal:
     return Decimal(value.replace(",", "."))
 
 
-def _to_rate(record: dict) -> ExchangeRate:
+def _to_rate(record: Dict[str, Any]) -> ExchangeRate:
     return ExchangeRate(
         date=date.fromisoformat(record["datum_primjene"]),
         currency_code=record["valuta"],
-        unit_value=record["jedinica"],
         buying_rate=_parse_decimal(record["kupovni_tecaj"]),
         median_rate=_parse_decimal(record["srednji_tecaj"]),
         selling_rate=_parse_decimal(record["prodajni_tecaj"]),
     )
```

### Comparing `hnbex-cli-2.0.0/hnbex/commands.py` & `hnbex_cli-2.1.0/hnbex/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,42 +14,41 @@
     pass
 
 
 def wrap(tag, text):
     return f"<{tag}>{text}</{tag}>"
 
 
-def daily(date, **kwargs):
+def daily(date, invert: bool, **kwargs):
     rates = fetch_daily(date)
 
     print_out(f"HNB exchange rates on <yellow>{date:%Y-%m-%d}</yellow>")
     print_out()
 
     if len(rates) == 0:
         print_out("No data found for given date")
         return
 
     def spread(rate):
         buy = rate.buying_rate
         sell = rate.selling_rate
-        if sell > 0:
-            diff = (sell - buy) / sell
+        if buy > 0:
+            diff = (buy - sell) / buy
             return f"{diff:.2%}"
         return ""
 
     data = [(
         wrap("yellow", rate.currency_code),
-        rate.unit_value,
-        rate.buying_rate,
-        rate.median_rate,
-        rate.selling_rate,
+        _maybe_invert(rate.buying_rate, invert),
+        _maybe_invert(rate.median_rate, invert),
+        _maybe_invert(rate.selling_rate, invert),
         spread(rate)
     ) for rate in rates]
 
-    headers = ["Currency", "Unit", "Buying", "Median", "Selling", "Spread"]
+    headers = ["Currency", "Buying", "Median", "Selling", "Spread"]
     print_table(headers, data)
 
 
 def _range_dates(start, end, days):
     if not start:
         start = end - timedelta(days=days - 1)
 
@@ -71,50 +70,49 @@
 
     if diff > 0:
         return f"<green>+{formatted}</green>"
 
     return f" {formatted}"
 
 
-def _range_lines(rates):
+def _range_lines(rates, invert):
     prev_median = None
     diff_median = None
 
     for rate in rates:
-        median = rate.median_rate
+        median = _maybe_invert(rate.median_rate, invert)
         diff_median = _diff(prev_median, median)
 
         yield(
             wrap("yellow", rate.date),
-            rate.unit_value,
-            rate.buying_rate,
-            rate.median_rate,
-            rate.selling_rate,
+            _maybe_invert(rate.buying_rate, invert),
+            _maybe_invert(rate.median_rate, invert),
+            _maybe_invert(rate.selling_rate, invert),
             diff_median,
         )
 
-        prev_median = rate.median_rate
+        prev_median = median
 
 
-def range(currency, start, end, days, **kwargs):
+def range(currency, start, end, days, invert, **kwargs):
     start_date, end_date = _range_dates(start, end, days)
     rates = fetch_range(currency, start_date, end_date)
 
     print_out(
         f"HNB exchange rates for <yellow>{currency}</yellow>",
         f"from <yellow>{start_date:%Y-%m-%d}</yellow>",
         f"to <yellow>{end_date:%Y-%m-%d}</yellow>\n"
     )
 
     if not rates:
         print_out("No data found for given date range")
         return
 
-    headers = ['Date', 'Unit', 'Buying', 'Median', 'Selling', 'Diff']
-    print_table(headers, _range_lines(rates))
+    headers = ['Date', 'Buying', 'Median', 'Selling', 'Diff']
+    print_table(headers, _range_lines(rates, invert))
 
 
 def _get_rate(date, currency):
     rates = fetch_daily(date, currency_code=currency)
 
     if rates:
         return rates[0]
@@ -122,37 +120,36 @@
     raise CommandError(f"Exchange rate for {currency} not found")
 
 
 def convert(amount, source_currency, target_currency, date, precision, value_only, **kwargs):
     if precision < 0:
         raise CommandError("Precision must be greater than 0.")
 
-    if source_currency != 'HRK' and target_currency != 'HRK':
-        raise CommandError("Either source or target currency must be HRK.")
+    if source_currency != 'EUR' and target_currency != 'EUR':
+        raise CommandError("Either source or target currency must be EUR.")
 
     if source_currency == target_currency:
         raise CommandError("Source and target currency are the same.")
 
-    if source_currency == 'HRK':
+    if source_currency == 'EUR':
         rate = _get_rate(date, target_currency)
-        result = amount / (rate.median_rate / rate.unit_value)
+        result = amount * rate.median_rate
     else:
         rate = _get_rate(date, source_currency)
-        result = amount * (rate.median_rate / rate.unit_value)
+        result = amount / rate.median_rate
 
-    exponent = Decimal(10) ** -precision
-    result = result.quantize(exponent)
+    result = quantize(result, precision)
 
     if value_only:
         print_out(result)
     else:
         print_out(f"{amount} {source_currency} = <green>{result} {target_currency}</green>\n")
         print_out(
-            f"Using the median rate {rate.unit_value} {rate.currency_code} =",
-            f"{rate.median_rate} HRK defined on {rate.date}"
+            f"Using the median rate 1 EUR =",
+            f"{rate.median_rate} {rate.currency_code} defined on {rate.date}"
         )
 
 
 def abspath(path):
     return join(realpath(dirname(__file__)), path)
 
 
@@ -187,7 +184,16 @@
 
 def _plot(script_file):
     try:
         call(['gnuplot', '-c', script_file.name, '-p'])
     except FileNotFoundError as ex:
         print_err(ex)
         raise CommandError("Charting failed. Do you have gnuplot installed?")
+
+
+def _maybe_invert(value: Decimal, invert: bool):
+    return quantize(1 / value, 6) if invert else value
+
+
+def quantize(decimal: Decimal, precision: int):
+    exponent = Decimal(10) ** -precision
+    return decimal.quantize(exponent)
```

### Comparing `hnbex-cli-2.0.0/hnbex/console.py` & `hnbex_cli-2.1.0/hnbex/console.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 import logging
 import re
 import sys
 
 from argparse import ArgumentParser, ArgumentTypeError
 from collections import namedtuple
 from datetime import date, datetime, timedelta
@@ -60,28 +58,38 @@
         "type": date_type,
     }),
     (["-d", "--days"], {
         "help": "number of days in the range (defaults to 30)",
         "type": int,
         "default": 30
     }),
+    (["-i", "--invert"], {
+        "help": "invert the exchange rate",
+        "action": "store_true",
+        "default": False,
+    }),
 ]
 
 
 COMMANDS = [
     Command(
         name="daily",
         description="Show daily exchange rates for all currencies",
         arguments=[
             (["date"], {
                 "help": "the lookup date",
                 "nargs": "?",
                 "type": date_type,
                 "default": date.today(),
             }),
+            (["-i", "--invert"], {
+                "help": "invert the exchange rate",
+                "action": "store_true",
+                "default": False,
+            }),
         ],
     ),
     Command(
         name="range",
         description="Show exchange rates for a single currency in the given date range",
         arguments=[
             (["currency"], {
@@ -115,17 +123,17 @@
                 "type": decimal_type,
             }),
             (["source_currency"], {
                 "help": "currency from which to convert",
                 "type": currency_type,
             }),
             (["target_currency"], {
-                "help": "currency code to which to convert (defaults to HRK)",
+                "help": "currency code to which to convert (defaults to EUR)",
                 "type": currency_type,
-                "default": "HRK",
+                "default": "EUR",
                 "nargs": "?",
             }),
             (["-d", "--date"], {
                 "help": "the lookup date (defaults to today)",
                 "type": date_type,
                 "default": date.today(),
             }),
@@ -156,19 +164,15 @@
         "action": 'store_true',
         "default": False,
     })
 ]
 
 
 def get_parser():
-    description = """
-        Exhange rates for Croatian Kuna (HRK) published by the Croatian National Bank (HNB).
-        Data fetched from hnb.ex, a service provided by Dobar Kod.
-    """
-
+    description = "Exhange rates published by the Croatian National Bank (HNB)."
     parser = ArgumentParser(prog='hnbex', description=description, epilog=CLIENT_WEBSITE)
     parser.add_argument('--no-color', action='store_true', help='don\'t use ANSI colors in output')
 
     subparsers = parser.add_subparsers(title="commands")
 
     for command in COMMANDS:
         sub = subparsers.add_parser(command.name, help=command.description)
```

### Comparing `hnbex-cli-2.0.0/hnbex/output.py` & `hnbex_cli-2.1.0/hnbex/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import sys
 import re
 
 
 START_CODES = {
     'red':     '\033[31m',
     'green':   '\033[32m',
```

### Comparing `hnbex-cli-2.0.0/hnbex_cli.egg-info/PKG-INFO` & `hnbex_cli-2.1.0/hnbex_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hnbex-cli
-Version: 2.0.0
+Version: 2.1.0
 Summary: CLI tool for displaying exchange rates for Croatian Kuna
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,14 +684,17 @@
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 HNB Exchange Rate CLI
 =====================
 
 Displays exchange rates for Croatian Kuna (HRK) from the Croatian National Bank
 (HNB). Data is fetched from the [HNB API](https://api.hnb.hr/).
```

