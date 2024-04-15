# Comparing `tmp/lanQ-1.2.tar.gz` & `tmp/lanQ-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanQ-1.2.tar", last modified: Tue Apr  9 06:12:22 2024, max compression
+gzip compressed data, was "lanQ-1.3.tar", last modified: Mon Apr 15 09:16:29 2024, max compression
```

## Comparing `lanQ-1.2.tar` & `lanQ-1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 06:12:22.206966 lanQ-1.2/
--rw-rw-rw-   0        0        0      192 2024-04-09 06:12:22.203970 lanQ-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5672 2024-04-08 09:38:17.000000 lanQ-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 06:12:22.202973 lanQ-1.2/lanQ.egg-info/
--rw-rw-rw-   0        0        0      192 2024-04-09 06:12:22.000000 lanQ-1.2/lanQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-04-09 06:12:22.000000 lanQ-1.2/lanQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 06:12:22.000000 lanQ-1.2/lanQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-09 06:12:22.000000 lanQ-1.2/lanQ.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 06:12:22.200978 lanQ-1.2/lanQ_rule/
--rw-rw-rw-   0        0        0        0 2024-03-19 08:32:28.000000 lanQ-1.2/lanQ_rule/__init__.py
--rw-rw-rw-   0        0        0     3465 2024-04-03 05:46:02.000000 lanQ-1.2/lanQ_rule/base.py
--rw-rw-rw-   0        0        0    10522 2024-04-08 09:12:55.000000 lanQ-1.2/lanQ_rule/common_rule.py
--rw-rw-rw-   0        0        0     1040 2024-04-08 09:12:55.000000 lanQ-1.2/lanQ_rule/const.py
--rw-rw-rw-   0        0        0      975 2024-04-03 05:52:18.000000 lanQ-1.2/lanQ_rule/model_rule.py
--rw-rw-rw-   0        0        0     1126 2024-04-03 05:46:02.000000 lanQ-1.2/lanQ_rule/prompt_rule.py
--rw-rw-rw-   0        0        0       42 2024-04-09 06:12:22.206966 lanQ-1.2/setup.cfg
--rw-rw-rw-   0        0        0      405 2024-04-08 09:29:55.000000 lanQ-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:16:29.360690 lanQ-1.3/
+-rw-rw-rw-   0        0        0      192 2024-04-15 09:16:29.358695 lanQ-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7459 2024-04-15 09:15:37.000000 lanQ-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 09:16:29.357697 lanQ-1.3/lanQ.egg-info/
+-rw-rw-rw-   0        0        0      192 2024-04-15 09:16:29.000000 lanQ-1.3/lanQ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-04-15 09:16:29.000000 lanQ-1.3/lanQ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 09:16:29.000000 lanQ-1.3/lanQ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-15 09:16:29.000000 lanQ-1.3/lanQ.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 09:16:29.355704 lanQ-1.3/lanQ_rule/
+-rw-rw-rw-   0        0        0        0 2024-03-19 08:32:28.000000 lanQ-1.3/lanQ_rule/__init__.py
+-rw-rw-rw-   0        0        0     3981 2024-04-11 02:54:19.000000 lanQ-1.3/lanQ_rule/base.py
+-rw-rw-rw-   0        0        0    16420 2024-04-15 08:37:04.000000 lanQ-1.3/lanQ_rule/common_rule.py
+-rw-rw-rw-   0        0        0     1471 2024-04-11 02:54:19.000000 lanQ-1.3/lanQ_rule/const.py
+-rw-rw-rw-   0        0        0      985 2024-04-15 08:37:04.000000 lanQ-1.3/lanQ_rule/model_rule.py
+-rw-rw-rw-   0        0        0     1156 2024-04-15 08:37:04.000000 lanQ-1.3/lanQ_rule/prompt_rule.py
+-rw-rw-rw-   0        0        0       42 2024-04-15 09:16:29.360690 lanQ-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      405 2024-04-15 09:15:46.000000 lanQ-1.3/setup.py
```

### Comparing `lanQ-1.2/lanQ_rule/base.py` & `lanQ-1.3/lanQ_rule/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -113,8 +113,19 @@
     chars_duped = numpy.sum(word_lengths * duplicated_grams)
     total_chars = numpy.sum(word_lengths)
 
     if total_chars == 0:
         return 0
 
     score = float(chars_duped / total_chars) * 100
-    return score
+    return score
+
+def get_real_text(text):
+    punc = ",;.!?:'\"/\\|_@#$%^&*~`+-=<>()[]{}·，；。！？：‘’“”、《》【】「」『』〔〕〈〉《》「」『』【】〖〗〘〙〚〛-—…～·‖ _│─┐┼┤"
+    pattern = "[" + re.escape(punc) + "]"
+    # punctuation_regex = r"[^\w\s]"
+    text = re.sub(pattern, "", text)
+
+    chinese_pattern = re.compile(r"[^\u4e00-\u9fa5]")
+    # 使用sub方法替换非汉字字符为空字符串
+    text = chinese_pattern.sub("", text)
+    return text
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lanQ-1.2/lanQ_rule/model_rule.py` & `lanQ-1.3/lanQ_rule/model_rule.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
 sys.path.append(os.path.dirname(__file__))
 
 from base import *
 from const import *
 
 def model_advertisement(content: str) -> dict:
-    """检查content内是否有广告."""
+    """check whether content has advertisement"""
     res = {'error_status': False}
     ad_list_en = ['deadlinesOrder', 'Kindly click on ORDER NOW to receive an']
     matches = re.findall('|'.join(ad_list_en), content)
     if matches:
         res["error_status"] = True
         res["error_type"] = ERROR_ADVERTISEMENT
         res['error_reason'] = matches
     return res
 
 def model_watermark(content: str) -> dict:
-    """检查content内是否有水印."""
+    """check whether content has watermark"""
     res = {'error_status': False}
     watermark_list = ['仩嗨亾笁潪能', '上s海h人r工g智z能n实s验y室s']
     matches = re.findall('|'.join(watermark_list), content)
     if matches:
         res["error_status"] = True
         res["error_type"] = ERROR_WATERMARK
         res['error_reason'] = '存在水印'
```

### Comparing `lanQ-1.2/lanQ_rule/prompt_rule.py` & `lanQ-1.3/lanQ_rule/prompt_rule.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 sys.path.append(os.path.dirname(__file__))
 
 from base import *
 from const import *
 
 def prompt_chinese_produce_english(prompt: str, prediction: str) -> dict:
-    """检查中文promt生成英文prediction."""
+    """check whether chinese prompt produce english prediction"""
     res = {'error_status': False}
     lan_prompt = langid.classify(prompt)[0]
     lan_prediction = langid.classify(prediction)[0]
     if lan_prompt == 'zh' and lan_prediction == 'en':
         res['error_status'] = True
         res['error_type'] = ERROR_CHINESE_PRODUCE_ENGLISH
         res['error_reason'] = '中文提示，生成英文内容'
     return res
 
 def prompt_english_produce_chinese(prompt: str, prediction: str) -> dict:
-    """检查英文promt生成中文prediction."""
+    """check whether english prompt produce chinese prediction"""
     res = {'error_status': False}
     lan_prompt = langid.classify(prompt)[0]
     lan_prediction = langid.classify(prediction)[0]
     if lan_prompt == 'en' and lan_prediction == 'zh':
         res['error_status'] = True
         res['error_type'] = ERROR_ENGLISH_PRODUCE_CHINESE
         res['error_reason'] = '英文提示，生成中文内容'
```

