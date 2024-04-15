# Comparing `tmp/mypylib-0.2.1.tar.gz` & `tmp/mypylib-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.2.1.tar", last modified: Thu Apr 11 10:20:26 2024, max compression
+gzip compressed data, was "mypylib-0.2.2.tar", last modified: Mon Apr 15 05:43:53 2024, max compression
```

## Comparing `mypylib-0.2.1.tar` & `mypylib-0.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-11 10:20:26.740391 mypylib-0.2.1/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-04-11 10:20:26.740103 mypylib-0.2.1/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2023-10-11 03:37:07.000000 mypylib-0.2.1/README.md
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-11 10:20:26.735008 mypylib-0.2.1/mypylib/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/MP_shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    51026 2024-04-11 10:19:20.000000 mypylib-0.2.1/mypylib/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3417 2024-01-25 14:54:07.000000 mypylib-0.2.1/mypylib/binance.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/binance_copy_bot.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/chdbif.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5984 2023-12-14 09:03:23.000000 mypylib-0.2.1/mypylib/crawler.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/crypto.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/finmind.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/libexcel.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/mvp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      157 2023-12-27 08:05:41.000000 mypylib-0.2.1/mypylib/my_random_proxy.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/option_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1109 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/rayin.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/shioaji_history_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/shioaji_kline.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    10696 2023-12-27 08:14:26.000000 mypylib-0.2.1/mypylib/sjtools.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/tLineNotify.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/ti.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-11 10:20:26.739558 mypylib-0.2.1/mypylib/tmpDevelopment/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/tmpDevelopment/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3085 2023-10-18 03:05:27.000000 mypylib-0.2.1/mypylib/tmpDevelopment/arping.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1892 2023-10-17 13:34:43.000000 mypylib-0.2.1/mypylib/tmpDevelopment/tmp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/tmpDevelopment/warrant_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2540 2024-03-19 15:35:40.000000 mypylib-0.2.1/mypylib/tplaysound.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8609 2023-10-16 13:50:29.000000 mypylib-0.2.1/mypylib/tredis.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    10029 2024-04-11 10:19:20.000000 mypylib-0.2.1/mypylib/warrant.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-11 10:20:26.736852 mypylib-0.2.1/mypylib.egg-info/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-04-11 10:20:26.000000 mypylib-0.2.1/mypylib.egg-info/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      748 2024-04-11 10:20:26.000000 mypylib-0.2.1/mypylib.egg-info/SOURCES.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2024-04-11 10:20:26.000000 mypylib-0.2.1/mypylib.egg-info/dependency_links.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2024-04-11 10:20:26.000000 mypylib-0.2.1/mypylib.egg-info/top_level.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2024-04-11 10:20:26.740472 mypylib-0.2.1/setup.cfg
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2023-10-11 03:37:07.000000 mypylib-0.2.1/setup.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-15 05:43:53.880657 mypylib-0.2.2/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-04-15 05:43:53.880272 mypylib-0.2.2/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2023-10-11 03:37:07.000000 mypylib-0.2.2/README.md
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-15 05:43:53.873740 mypylib-0.2.2/mypylib/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/MP_shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    51079 2024-04-15 05:42:08.000000 mypylib-0.2.2/mypylib/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3417 2024-01-25 14:54:07.000000 mypylib-0.2.2/mypylib/binance.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/binance_copy_bot.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/chdbif.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5984 2023-12-14 09:03:23.000000 mypylib-0.2.2/mypylib/crawler.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/crypto.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/finmind.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/libexcel.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/mvp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      157 2023-12-27 08:05:41.000000 mypylib-0.2.2/mypylib/my_random_proxy.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/option_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1109 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/rayin.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/shioaji_history_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/shioaji_kline.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    10696 2023-12-27 08:14:26.000000 mypylib-0.2.2/mypylib/sjtools.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/tLineNotify.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/ti.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-15 05:43:53.879556 mypylib-0.2.2/mypylib/tmpDevelopment/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/tmpDevelopment/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3085 2023-10-18 03:05:27.000000 mypylib-0.2.2/mypylib/tmpDevelopment/arping.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1892 2023-10-17 13:34:43.000000 mypylib-0.2.2/mypylib/tmpDevelopment/tmp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/tmpDevelopment/warrant_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2540 2024-03-19 15:35:40.000000 mypylib-0.2.2/mypylib/tplaysound.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8609 2023-10-16 13:50:29.000000 mypylib-0.2.2/mypylib/tredis.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    10618 2024-04-15 05:41:25.000000 mypylib-0.2.2/mypylib/warrant.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-15 05:43:53.876632 mypylib-0.2.2/mypylib.egg-info/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-04-15 05:43:53.000000 mypylib-0.2.2/mypylib.egg-info/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      748 2024-04-15 05:43:53.000000 mypylib-0.2.2/mypylib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2024-04-15 05:43:53.000000 mypylib-0.2.2/mypylib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2024-04-15 05:43:53.000000 mypylib-0.2.2/mypylib.egg-info/top_level.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2024-04-15 05:43:53.880840 mypylib-0.2.2/setup.cfg
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2023-10-11 03:37:07.000000 mypylib-0.2.2/setup.py
```

### Comparing `mypylib-0.2.1/README.md` & `mypylib-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/MP_shioaji_ticks.py` & `mypylib-0.2.2/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/__init__.py` & `mypylib-0.2.2/mypylib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,17 +89,18 @@
     '2024/01/02: 0.1.95 Update get_punishment_list()',
     '2024/03/11: 0.1.96 修正處置股資料。必須要看是否在期限內',
     '2024/03/13: 0.1.97 fix get_punishment_list()',
     '2024/03/23: 0.1.98 add warrant_bible_convert_to_c_need()',
     '2024/03/24: 0.1.99 modify warrant_bible_convert_to_c_need() and save warrant_bible.txt',
     '2024/03/27: 0.2.00 fix get_punishment_list() date bug ',
     '2024/04/11: 0.2.01 fix warrant_bible_convert_to_c_need() bug',
+    '2024/04/15: 0.2.02 add warrant_bible_do_all()',
 }
 
-__version__ = '0.2.01'
+__version__ = '0.2.02'
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
 
 path_cronlog = 'cronlog'
```

### Comparing `mypylib-0.2.1/mypylib/binance.py` & `mypylib-0.2.2/mypylib/binance.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/binance_copy_bot.py` & `mypylib-0.2.2/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/chdbif.py` & `mypylib-0.2.2/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/crawler.py` & `mypylib-0.2.2/mypylib/crawler.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/crypto.py` & `mypylib-0.2.2/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/finmind.py` & `mypylib-0.2.2/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/libexcel.py` & `mypylib-0.2.2/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/mvp.py` & `mypylib-0.2.2/mypylib/mvp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/option_test.py` & `mypylib-0.2.2/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/rayin.py` & `mypylib-0.2.2/mypylib/rayin.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/shioaji_history_ticks.py` & `mypylib-0.2.2/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/shioaji_kline.py` & `mypylib-0.2.2/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/shioaji_ticks.py` & `mypylib-0.2.2/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/sjtools.py` & `mypylib-0.2.2/mypylib/sjtools.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/tLineNotify.py` & `mypylib-0.2.2/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/ti.py` & `mypylib-0.2.2/mypylib/ti.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/tmpDevelopment/arping.py` & `mypylib-0.2.2/mypylib/tmpDevelopment/arping.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/tmpDevelopment/tmp.py` & `mypylib-0.2.2/mypylib/tmpDevelopment/tmp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.2.2/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/tplaysound.py` & `mypylib-0.2.2/mypylib/tplaysound.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/tredis.py` & `mypylib-0.2.2/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/mypylib/warrant.py` & `mypylib-0.2.2/mypylib/warrant.py`

 * *Files 7% similar despite different names*

```diff
@@ -142,30 +142,29 @@
         code = dict_warrant_to_info[x]['標的代碼']
         dict_stock_to_warrant[code].append(x)
 
     # print(stock_warrant_map)
     return dict_warrant_to_info, dict_stock_to_warrant
 
 
-def add_new_issued_warrant_to_bible(dict_warrant_to_info, dict_stock_to_warrant, list_new_warrants, date_to_file):
+def add_new_issued_warrant_to_bible(dict_warrant_to_info, dict_stock_to_warrant, list_new_warrants):
     # ('T', '06227P', '南電麥證26售01', '認售', '8046', '南電', '111/12/22')
     # ('N', '06228P', '臺股指麥證26售15', '認售', '加權指數', '加權指數', '111/12/22')
 
     for x in list_new_warrants:
-        if x[6][-5:] != date_to_file[-5:]:
-            # print(x[3][-5:], date_to_filte[-5:])
-            continue
         if x[0] == 'N':
             continue
-
         if x[3] != '認購':
             continue
-
         if x[1] not in dict_warrant_to_info.keys():
-            print(f'新權證: {x[1]} {x[2]} {date_to_file}')
+            year, month, day = x[6].split('/')
+            year = int(year) + 1911
+            date_to_file = f'{year}/{month}/{day}'
+
+            print(f'新權證: {x[1]} {x[2]} {x[6]} {date_to_file}')
 
             dict_warrant_to_info[x[1]] = {
                 '權證名稱': x[2],
                 '發行券商': x[2],
                 '權證價格': 0,
                 '權證漲跌': 0,
                 '權證漲跌幅': 0,
@@ -207,52 +206,72 @@
                 'Volume': 0
             }
 
             dict_stock_to_warrant[x[4]].append(x[1])
     return dict_warrant_to_info, dict_stock_to_warrant
 
 
-def warrant_bible_convert_to_c_need(file_to_convert=None):
-    if file_to_convert is None:
-        files = os.listdir(f'{expanduser("~")}/warrant')
-        files.sort(reverse=True)
-        file = ''
-        for file in files:
-            if file.endswith('.xls'):
-                break
-        file_to_convert = f'{expanduser("~")}/warrant/{file}'
-
-    print(f'讀取權證達人寶典: {file_to_convert}')
-    dict_warrant_to_info, dict_stock_to_warrant = read_warrant_bible(file_to_convert)
-    date_to_filte = datetime.datetime.today().strftime('%Y/%m/%d')
-    list_new_warrants = get_new_warrant_list()
-
-    dict_warrant_to_info, dict_stock_to_warrant = add_new_issued_warrant_to_bible(dict_warrant_to_info,
-                                                                                  dict_stock_to_warrant,
-                                                                                  list_new_warrants,
-                                                                                  date_to_filte)
-
-    target_file = f'{file_to_convert.split(".")[0]}.txt'
+def warrant_bible_convert_to_c_need(dict_warrant_to_info):
+    target_file = f'{expanduser("~")}/warrant/warrant_bible.txt'
     with open(target_file, "w+") as fp:
         for warrant in dict_warrant_to_info:
             fp.write(f'{warrant}\t{dict_warrant_to_info[warrant]["標的代碼"]}\t{dict_warrant_to_info[warrant]["認購/售類別"]}\n')
 
-    path_dir = os.path.dirname(target_file)
-    file_name = os.path.basename(target_file)
-    shutil.copy(target_file, f'{path_dir}/warrant_bible.txt')
+
+def download_latest_warrant_bible():
+    day_now = datetime.datetime.now()
+
+    while True:
+        str_date = day_now.strftime('%Y-%m-%d')
+        target_file = f'{expanduser("~")}/warrant/warrant-{str_date}.xls'
+        url = f'http://iwarrant-mobile.capital.com.tw/wdataV2/canonical/capital-newvol/%E6%AC%8A%E8%AD%89%E9%81%94%E4%BA%BA%E5%AF%B6%E5%85%B8_NEWVOL_{str_date}.xls'
+        print(f'下載權證達人寶典: {url}')
+
+        r = requests.get(url, headers={'User-agent': 'Mozilla/5.0'}, stream=True)
+        if r.status_code == 200:
+            with open(target_file, 'wb') as f:
+                f.write(r.content)
+            break
+        else:
+            print(f'找不到 {url}')
+            day_now -= datetime.timedelta(days=1)
+
+
+def get_last_warrant_bible_date():
+    files = os.listdir(f'{expanduser("~")}/warrant')
+    files.sort(reverse=True)
+    file = ''
+    for file in files:
+        if file.startswith('warrant') and file.endswith('.xls'):
+            bool_found = True
+            # warrant-2024-04-12.xls
+            return file[8:18]
+    return None
+
+
+def warrant_bible_do_all():
+    import datetime
+    download_latest_warrant_bible()
+    date_str = get_last_warrant_bible_date()
+    dict_warrant_to_info, dict_stock_to_warrant = read_warrant_bible(f'{expanduser("~")}/warrant/warrant-{date_str}.xls')
+    list_new_warrants = get_new_warrant_list()
+    dict_warrant_to_info, dict_stock_to_warrant = add_new_issued_warrant_to_bible(dict_warrant_to_info,
+                                                                                  dict_stock_to_warrant,
+                                                                                  list_new_warrants)
+    warrant_bible_convert_to_c_need(dict_warrant_to_info)
 
 
 if __name__ == '__main__':
     import datetime
 
-    date_to_file = datetime.datetime.today().strftime('%Y/%m/%d')
+    download_latest_warrant_bible()
 
-    # print(date_to_filte)
+    # 2024-04-12
+    date_str = get_last_warrant_bible_date()
 
-    dict_warrant_to_info, dict_stock_to_warrant = read_warrant_bible(f'{expanduser("~")}/warrant/warrant-2024-03-22.xls')
+    dict_warrant_to_info, dict_stock_to_warrant = read_warrant_bible(f'{expanduser("~")}/warrant/warrant-{date_str}.xls')
     list_new_warrants = get_new_warrant_list()
 
     dict_warrant_to_info, dict_stock_to_warrant = add_new_issued_warrant_to_bible(dict_warrant_to_info,
                                                                                   dict_stock_to_warrant,
-                                                                                  list_new_warrants,
-                                                                                  date_to_file)
-    warrant_bible_convert_to_c_need()
+                                                                                  list_new_warrants)
+    warrant_bible_convert_to_c_need(dict_warrant_to_info)
```

### Comparing `mypylib-0.2.1/mypylib.egg-info/SOURCES.txt` & `mypylib-0.2.2/mypylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.1/setup.py` & `mypylib-0.2.2/setup.py`

 * *Files identical despite different names*

