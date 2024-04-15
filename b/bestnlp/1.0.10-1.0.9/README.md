# Comparing `tmp/bestnlp-1.0.10-py3-none-any.whl.zip` & `tmp/bestnlp-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 1912609 bytes, number of entries: 10
+Zip file size: 1912584 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      239 b- defN 24-Apr-03 06:50 bestnlp/__init__.py
 -rw-r--r--  2.0 unx  5071852 b- defN 24-Mar-29 09:38 bestnlp/dict.txt
 -rw-r--r--  2.0 unx     7694 b- defN 24-Apr-10 02:48 bestnlp/new_word_discovery.py
--rw-r--r--  2.0 unx     4564 b- defN 24-Apr-15 06:22 bestnlp/similar_word_discovery.py
+-rw-r--r--  2.0 unx     4477 b- defN 24-Apr-12 02:25 bestnlp/similar_word_discovery.py
 -rw-r--r--  2.0 unx     4004 b- defN 24-Mar-29 09:39 bestnlp/similar_word_discovery_embedding.py
 -rw-r--r--  2.0 unx      958 b- defN 24-Apr-09 10:58 bestnlp/utils.py
--rw-r--r--  2.0 unx      246 b- defN 24-Apr-15 06:23 bestnlp-1.0.10.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 06:23 bestnlp-1.0.10.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-15 06:23 bestnlp-1.0.10.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      799 b- defN 24-Apr-15 06:23 bestnlp-1.0.10.dist-info/RECORD
-10 files, 5090456 bytes uncompressed, 1911251 bytes compressed:  62.5%
+-rw-r--r--  2.0 unx      245 b- defN 24-Apr-12 02:40 bestnlp-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 02:40 bestnlp-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-12 02:40 bestnlp-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      795 b- defN 24-Apr-12 02:40 bestnlp-1.0.9.dist-info/RECORD
+10 files, 5090364 bytes uncompressed, 1911234 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: bestnlp/similar_word_discovery_embedding.py
 Comment: 
 
 Filename: bestnlp/utils.py
 Comment: 
 
-Filename: bestnlp-1.0.10.dist-info/METADATA
+Filename: bestnlp-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: bestnlp-1.0.10.dist-info/WHEEL
+Filename: bestnlp-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: bestnlp-1.0.10.dist-info/top_level.txt
+Filename: bestnlp-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: bestnlp-1.0.10.dist-info/RECORD
+Filename: bestnlp-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bestnlp/similar_word_discovery.py

```diff
@@ -9,16 +9,16 @@
 
     click dataframe
     time  keyword  user_id  item_id
     """
     def process_search(self, search_df, threshold=10, time_name="time", user_id_name="user_id", keyword_name="keyword",):
         #搜索行为
         di = dict()
-        search_df[keyword_name] = search_df[keyword_name].apply(lambda x: x.strip().lower())
-        search_df = search_df[~((search_df[keyword_name].isnull()) | (search_df[keyword_name]==""))]
+        search_df[keyword_name] = search_df[keyword_name].apply(lambda x: x.strip())
+        search_df = search_df[~search_df[keyword_name].isnull()]
         df = search_df.sort_values(time_name)
         df = df.groupby(user_id_name)[keyword_name].agg(list).reset_index()
         for keyword in df[keyword_name].tolist():
             if len(keyword) >= 2:
                 for i in range(len(keyword) - 1):
                     if keyword[i] == keyword[i + 1]: continue
                     key = frozenset([keyword[i], keyword[i + 1]])
@@ -29,16 +29,16 @@
                 res[key] = value
         return res
 
 
     def process_click(self, click_df, threshold=10, time_name="time", user_id_name="user_id", keyword_name="keyword", item_id_name="item_id"):
         #点击行为
         #同一个商品点击等行为对应的搜索词
-        click_df[keyword_name] = click_df[keyword_name].apply(lambda x: x.strip().lower())
-        click_df = click_df[~((click_df[keyword_name].isnull()) | (click_df[keyword_name]==""))]
+        click_df[keyword_name] = click_df[keyword_name].apply(lambda x: x.strip())
+        click_df = click_df[~click_df[keyword_name].isnull()]
         act_df = click_df.sort_values(time_name).drop_duplicates([user_id_name, keyword_name, item_id_name])
         df = act_df.groupby(item_id_name)[keyword_name].agg(list).reset_index()
         di = dict()
         for keyword in df[keyword_name].tolist():
             if len(keyword) >= 2:
                 for key1 in keyword:
                     for key2 in keyword:
```

