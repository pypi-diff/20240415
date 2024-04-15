# Comparing `tmp/event_time_format-1.0.2-py3-none-any.whl.zip` & `tmp/event_time_format-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 13697 bytes, number of entries: 8
+Zip file size: 14435 bytes, number of entries: 8
 -rw-r--r--  2.0 unx    33241 b- defN 24-Mar-16 03:37 event_time_format/Test_event_time_format.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-16 03:44 event_time_format/__init__.py
--rw-r--r--  2.0 unx    32507 b- defN 24-Mar-16 03:37 event_time_format/event_time_format.py
--rw-r--r--  2.0 unx     1507 b- defN 24-Mar-18 00:47 event_time_format-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1196 b- defN 24-Mar-18 00:47 event_time_format-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-18 00:47 event_time_format-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-Mar-18 00:47 event_time_format-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      716 b- defN 24-Mar-18 00:47 event_time_format-1.0.2.dist-info/RECORD
-8 files, 69277 bytes uncompressed, 12429 bytes compressed:  82.1%
+-rw-r--r--  2.0 unx    33660 b- defN 24-Apr-15 12:06 event_time_format/event_time_format.py
+-rw-r--r--  2.0 unx     1507 b- defN 24-Apr-15 12:13 event_time_format-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1480 b- defN 24-Apr-15 12:13 event_time_format-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 12:13 event_time_format-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-Apr-15 12:13 event_time_format-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      716 b- defN 24-Apr-15 12:13 event_time_format-1.0.3.dist-info/RECORD
+8 files, 70714 bytes uncompressed, 13167 bytes compressed:  81.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: event_time_format/__init__.py
 Comment: 
 
 Filename: event_time_format/event_time_format.py
 Comment: 
 
-Filename: event_time_format-1.0.2.dist-info/LICENSE
+Filename: event_time_format-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: event_time_format-1.0.2.dist-info/METADATA
+Filename: event_time_format-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: event_time_format-1.0.2.dist-info/WHEEL
+Filename: event_time_format-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: event_time_format-1.0.2.dist-info/top_level.txt
+Filename: event_time_format-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: event_time_format-1.0.2.dist-info/RECORD
+Filename: event_time_format-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## event_time_format/event_time_format.py

```diff
@@ -5,16 +5,60 @@
 # 2014-11-19
 #
 
 import re
 import logging
 import time
 import arrow
+import requests
+import numpy as np
+import pandas as pd
+import tensorflow as tf
+from bs4 import BeautifulSoup
+
+
+
 #import json
 
+def getUtcTime():
+    url = 'http://worldtimeapi.org/api/timezone/Etc/UTC'
+    response = requests.get(url)
+    if response.status_code == 200:
+        data = response.json()
+        return data['datetime']
+    else:
+        print("Failed to retrieve UTC time.")
+        return None
+
+def numpyTime():
+    arr = np.array([1, 2, 3])
+    arr_times_2 = arr * 2
+    return arr_times_2
+
+def pandasEvent():
+    data = {'Name': ['Alice', 'Bob', 'Charlie'], 'Age': [25, 30, 35]}
+    df = pd.DataFrame(data)
+    print(df)
+
+def testTf(x_train, y_train):
+    model = tf.keras.Sequential([
+        tf.keras.layers.Dense(64, activation='relu', input_shape=(784,)),
+        tf.keras.layers.Dense(10, activation='softmax')
+    ])
+    model.compile(optimizer='adam',
+                loss='sparse_categorical_crossentropy',
+                metrics=['accuracy'])
+
+    model.fit(x_train, y_train, epochs=5)
+
+def testBs4():
+    html_doc = "<html><body><p>Hello, World!</p></body></html>"
+    soup = BeautifulSoup(html_doc, 'html.parser')
+    print(soup.p.text)
+
 #
 # weekday base on 0 (星期一)
 #
 
 def always(start_time, end_time):
     """is always
     start_day: YYYY-MM-DD or YYYY-MM-DD HH:mm:ss
```

## Comparing `event_time_format-1.0.2.dist-info/LICENSE` & `event_time_format-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `event_time_format-1.0.2.dist-info/METADATA` & `event_time_format-1.0.3.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-time-format
-Version: 1.0.2
+Version: 1.0.3
 Summary: event time format
 Home-page: https://github.com/errord/EventTimeFormat
 Author: errord
 Author-email: errord@gmail.com
 License: BSD License
 Project-URL: Source, https://github.com/errord/EventTimeFormat
 Platform: all
@@ -18,15 +18,25 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 Requires-Dist: arrow (>=1.1.0)
+Requires-Dist: requests (>=2.20.1)
+Requires-Dist: numpy (>=1.21.0)
+Requires-Dist: pandas (>=1.3.3)
+Requires-Dist: tensorflow (>=2.5.1)
+Requires-Dist: bs4 (>=0.0.2)
 
 # Readme
 格式化时间，通过多种中文格式显示
 
 # EventTimeFormat
 时间格式化 ： 11月19日 ~ 2015年1月30日 每周三，日 09:30-22:30 | 11月19日 ~ 2015年1月30日 每周三，日 全天 |  全年 每周四 10:30-21:00 |  每周四 10:30-21:00
 
+# pypi发布
+```shell
+python3 setup.py sdist bdist_wheel
+twine upload dist/event_time_format-1.0.x-py3-none-any.whl
+```
```

## Comparing `event_time_format-1.0.2.dist-info/RECORD` & `event_time_format-1.0.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 event_time_format/Test_event_time_format.py,sha256=SjspbGjUhGNWMkGtxP3jRH4QOBeJjF6QJ30-JLeJqqk,33241
 event_time_format/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-event_time_format/event_time_format.py,sha256=gUx0xL1TLe4M3a6DUecR6bKBGg-ZJ5cblMcVutyFVHU,32507
-event_time_format-1.0.2.dist-info/LICENSE,sha256=GG8m2F1Jso-pK53zaj4MtBT0xOMA25ih7DP5KshMQnM,1507
-event_time_format-1.0.2.dist-info/METADATA,sha256=cElv1gcw8SIe7ZgkOJ43nk7MXDPbbr0zwQ8Y2gNKHSw,1196
-event_time_format-1.0.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-event_time_format-1.0.2.dist-info/top_level.txt,sha256=pesUy3lblp-iQpd-4IM5NBtj5xilsVZlZsMW-rvrOPI,18
-event_time_format-1.0.2.dist-info/RECORD,,
+event_time_format/event_time_format.py,sha256=C8JJ9GkmFJo1Dt3xW7KHhFqjT8xpc326DhGfoPbPPps,33660
+event_time_format-1.0.3.dist-info/LICENSE,sha256=GG8m2F1Jso-pK53zaj4MtBT0xOMA25ih7DP5KshMQnM,1507
+event_time_format-1.0.3.dist-info/METADATA,sha256=BV0pV_vVOeJXfBk9HKEn_VuroGSoXNNjAIXZ9fb-aH4,1480
+event_time_format-1.0.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+event_time_format-1.0.3.dist-info/top_level.txt,sha256=pesUy3lblp-iQpd-4IM5NBtj5xilsVZlZsMW-rvrOPI,18
+event_time_format-1.0.3.dist-info/RECORD,,
```

