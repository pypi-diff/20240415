# Comparing `tmp/glook-0.0.8-py3-none-any.whl.zip` & `tmp/glook-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 16194 bytes, number of entries: 12
+Zip file size: 16198 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat     2776 b- defN 24-Apr-14 16:10 glook/GLook.py
 -rw-rw-rw-  2.0 fat       51 b- defN 24-Mar-25 17:39 glook/__init__.py
 -rw-rw-rw-  2.0 fat      339 b- defN 24-Mar-25 18:24 glook/cli.py
 -rw-rw-rw-  2.0 fat     3698 b- defN 24-Apr-14 17:22 glook/pages/1_General_Data_Insights.py
 -rw-rw-rw-  2.0 fat    17728 b- defN 24-Apr-14 15:18 glook/pages/2_Univariate_Analysis.py
 -rw-rw-rw-  2.0 fat     7771 b- defN 24-Apr-14 11:53 glook/pages/3_Bivariate_Analysis.py
 -rw-rw-rw-  2.0 fat     7596 b- defN 24-Mar-28 17:23 glook/pages/4_Trivariate_Analysis.py
--rw-rw-rw-  2.0 fat     4139 b- defN 24-Apr-15 16:56 glook-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 16:56 glook-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-15 16:56 glook-0.0.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-15 16:56 glook-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      967 b- defN 24-Apr-15 16:56 glook-0.0.8.dist-info/RECORD
-12 files, 45201 bytes uncompressed, 14568 bytes compressed:  67.8%
+-rw-rw-rw-  2.0 fat     4101 b- defN 24-Apr-15 18:03 glook-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 18:03 glook-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-15 18:03 glook-0.0.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-15 18:03 glook-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      967 b- defN 24-Apr-15 18:03 glook-0.0.9.dist-info/RECORD
+12 files, 45163 bytes uncompressed, 14572 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: glook/pages/3_Bivariate_Analysis.py
 Comment: 
 
 Filename: glook/pages/4_Trivariate_Analysis.py
 Comment: 
 
-Filename: glook-0.0.8.dist-info/METADATA
+Filename: glook-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: glook-0.0.8.dist-info/WHEEL
+Filename: glook-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: glook-0.0.8.dist-info/entry_points.txt
+Filename: glook-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: glook-0.0.8.dist-info/top_level.txt
+Filename: glook-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: glook-0.0.8.dist-info/RECORD
+Filename: glook-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `glook-0.0.8.dist-info/METADATA` & `glook-0.0.9.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: glook
-Version: 0.0.8
+Version: 0.0.9
 Summary: Auto EDA.
 Home-page: https://github.com/gaurang157/glook
 Author: Gaurang Ingle
 Author-email: gaurang.ingle@gmail.com
-Maintainer: ['Gaurang Ingle', 'Sharat Chandra Manikonda']
-Maintainer-email: [('Gaurang Ingle', 'gaurang.ingle@gmail.com'), ('Sharat Chandra Manikonda', 'manikondasharat@gmail.com')]
+Maintainer: dict_keys(['Gaurang Ingle', 'Sharat Chandra Manikonda'])
+Maintainer-email: ['gaurang.ingle@gmail.com', 'manikondasharat@gmail.com']
 License: MIT
 Project-URL: Bug Reports, https://github.com/gaurang157/glook/issues
 Project-URL: Source, https://github.com/gaurang157/glook
 Project-URL: Documentation, https://github.com/gaurang157/glook/blob/main/README.md
 Project-URL: Say Thanks!, https://github.com/gaurang157/glook/issues/new?assignees=&labels=&template=thanks.yml
 Keywords: AutoEDA,Exploratory Data Analysis,Data Visualization,GUI,CLI,Python,Streamlit,CLI interface,UI interface
 Classifier: Programming Language :: Python :: 3
```

## Comparing `glook-0.0.8.dist-info/RECORD` & `glook-0.0.9.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 glook/GLook.py,sha256=8ppiVKtPyvA29zKzbQMNHzsM37EltchjN70XrB4AcvA,2776
 glook/__init__.py,sha256=8NahmY4XQHJYMnFDvkZnHpjVBHwxrYrnDFlTTuyXbB0,51
 glook/cli.py,sha256=zBVCZyNNyRj_Zy4Tdnbrb1TrgRhEqAEEdZbk_vrLmi4,339
 glook/pages/1_General_Data_Insights.py,sha256=btHs2krtxH-H2MdX_x0hLnp8NR38dYvNnVdnNNjZosc,3698
 glook/pages/2_Univariate_Analysis.py,sha256=iQd1MsSFCdtIFU6coQBN-T9FWTVoVUA_Baf1evwjanA,17728
 glook/pages/3_Bivariate_Analysis.py,sha256=0fyPduQDUnlrfYk48YTV3JkxCaTxBjZANfzfPZMjllg,7771
 glook/pages/4_Trivariate_Analysis.py,sha256=Fhkmzqur1xBLPBviyI8kQeeFQbQYAhKwsOLw4E83Hs8,7596
-glook-0.0.8.dist-info/METADATA,sha256=AjEDAHL46wC16YhkK4XlxnJeOMlCi36NSBSephkZ3F0,4139
-glook-0.0.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-glook-0.0.8.dist-info/entry_points.txt,sha256=7q8WVzTgIl4vX4wJgctmfdJckoB5yPtI0p3hqAQSiFA,38
-glook-0.0.8.dist-info/top_level.txt,sha256=2wtpfrIqw9VT_LFDxpI77DArLrUaNjWxyClToM3P9WE,6
-glook-0.0.8.dist-info/RECORD,,
+glook-0.0.9.dist-info/METADATA,sha256=60rIh_SXYzj2ivCZh6t4albrSN9lbhqMR5c3wf1T7CY,4101
+glook-0.0.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+glook-0.0.9.dist-info/entry_points.txt,sha256=7q8WVzTgIl4vX4wJgctmfdJckoB5yPtI0p3hqAQSiFA,38
+glook-0.0.9.dist-info/top_level.txt,sha256=2wtpfrIqw9VT_LFDxpI77DArLrUaNjWxyClToM3P9WE,6
+glook-0.0.9.dist-info/RECORD,,
```

