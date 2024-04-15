# Comparing `tmp/secretaries-0.0.1.7.tar.gz` & `tmp/secretaries-0.0.1.8.tar.gz`

## Comparing `secretaries-0.0.1.7.tar` & `secretaries-0.0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 secretaries-0.0.1.7/src/secretaries/__init__.py
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 secretaries-0.0.1.7/src/secretaries/patterns.py
--rwxr-xr-x   0        0        0    27022 2020-02-02 00:00:00.000000 secretaries-0.0.1.7/src/secretaries/secretary.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 secretaries-0.0.1.7/src/secretaries/starter_kit_safe_words_en.csv
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 secretaries-0.0.1.7/src/secretaries/startkit_ickenamn_se.csv
--rw-r--r--   0        0        0    12330 2020-02-02 00:00:00.000000 secretaries-0.0.1.7/src/secretaries/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 secretaries-0.0.1.7/tests/test.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 secretaries-0.0.1.7/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 secretaries-0.0.1.7/LICENSE
--rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 secretaries-0.0.1.7/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 secretaries-0.0.1.7/pyproject.toml
--rw-r--r--   0        0        0    16813 2020-02-02 00:00:00.000000 secretaries-0.0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/src/secretaries/__init__.py
+-rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/src/secretaries/patterns.py
+-rwxr-xr-x   0        0        0    27321 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/src/secretaries/secretary.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/src/secretaries/starter_kit_safe_words_en.csv
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/src/secretaries/startkit_ickenamn_se.csv
+-rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/src/secretaries/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/tests/test.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/LICENSE
+-rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/README.md
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/PKG-INFO
```

### Comparing `secretaries-0.0.1.7/src/secretaries/patterns.py` & `secretaries-0.0.1.8/src/secretaries/patterns.py`

 * *Files identical despite different names*

### Comparing `secretaries-0.0.1.7/src/secretaries/secretary.py` & `secretaries-0.0.1.8/src/secretaries/secretary.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         ner = True,
         corpus = True, 
         lang = 'se',
         names = list(),
         ambiguous = list(),
         masks = list(),
         single_text_mode = False,
+        strict = True,
         min_n_persons = 100, 
         max_sequence_length = 3, 
         remove_html = True,
         preserve_linebreaks = True,
         model_name = 'KB/bert-base-swedish-cased-ner'):
     """Main function for running the secretary
     
@@ -75,14 +76,16 @@
         Optional runtime list of tokens to add to the corpus as names
     ambiguous : Optional[list] 
         Optional runtime list of tokens not considered names, to exclude from the corpus
     masks : Optional[list]
         Optional runtime list of single or multi token words to hide from the algorithm and thus preserve from the substitutions
     single_text_mode : Optional[bool]
         Optionally return a single text. May be useful for setting up an api. 
+    strict : Optional[bool]
+        If True, disallow the splitting of text mid-sentence, when two adjacent punctuation marks are further apart than the 512 max token length of BERT models. Set to False as needed, when there is not enough punctuation in your text.
     min_n_persons : Optional[int]
         An optional frequency threshold for corpus tokens. At present only available in Swedish. Defaults to 100. 
     max_sequence_length : Optional[int] 
         Given a list L and a text T, there are two ways of finding which tokens in L are present in T. One is to split T into parts of 1 through n token sequences and check whether each sequence is present in L. This makes sense for shorter sequences, mainly single token words. When searching for longer sequences, you end up with a lot of combinations of 1 through n tokens. It then becomes more efficient to iterate though L and do a literal search for it in T. The max_sequence_length arguments controls at what sequence length the latter method is used. Defaults to 3, meaning sequences of at most 3 tokens will be extracted from each text. You may opt for a lower setting depending on computational resources. A higher setting might make sense if you have a very long list of multi-word masks.  
     remove_html : Optional[bool]
         Whether or not to remove html tags. Defaults to True.
     preserve_linebreaks : Optional[bool]
@@ -150,15 +153,15 @@
     if preserve_linebreaks: 
         df = df.with_columns(pl.col(text_column) \
                              .str.replace_all(r"\r|\n", tags["linebreak_placeholder"]))
 
     # Pre-processing in eager mode:
     # Split text into parts of at most 512 tokens (the BERT model word limit)
     # NB: punctuation also counts as tokens
-    insert_splits = partial(insert_splits_, 512, tags["split_token"])
+    insert_splits = partial(insert_splits_, 512, tags["split_token"], strict)
     df = df.collect() \
         .with_columns(pl.col(text_column).map_elements(insert_splits).keep_name()) \
         .with_columns(pl.col(text_column).str.split(tags["split_token"]).keep_name()) \
         .with_columns(pl.col(text_column).list.lengths().alias('n_splits')) \
         .lazy()
 
     # Remove brackets with numbers (eg <1>, <<5>>, <<<<<25>>>>>) so that
```

### Comparing `secretaries-0.0.1.7/src/secretaries/startkit_ickenamn_se.csv` & `secretaries-0.0.1.8/src/secretaries/startkit_ickenamn_se.csv`

 * *Files identical despite different names*

### Comparing `secretaries-0.0.1.7/src/secretaries/utils.py` & `secretaries-0.0.1.8/src/secretaries/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,53 +169,61 @@
 
     txt = x[text_column]
     name_tag = '[ ' + tags['name'] + ' ]'
     for token in x['names_from_corpus']:
         txt = re.sub(r'(?i)\b' + re.escape(token) + r'\b', name_tag, txt)
     return txt
 
-def insert_splits_(split_length, split_token, text):
+def insert_splits_(split_length, split_token, strict, text):
     """Splits a text into chunks of at most split_length tokens. Useful for constraints like the 512 word limit of BERT models."""
 
     tokens = re.split(pattern = r'\b', string = text)
     # If the number of tokens is less than split_length, do nothing
     if len(tokens) <= split_length:
         return(text)
 
     is_punctuation = list(map(bool, [re.search(r"^[?.!]+\s?", t) for t in tokens]))
     if not any(is_punctuation):
         # If no [?.!] present, split by comma.
         is_comma = list(map(bool, [re.search(r"^,+\s?", t) for t in tokens]))
-        print(sum(is_comma))
         if any(is_comma):
             is_punctuation = is_comma
             warnings.warn('No punctuations in text, splitting by comma instead.')
-            print(is_punctuation)
         else:
-            # If no punctuation present, do not split text
-            warnings.warn('No punctuation or comma in text - cannot split accordingly. Put some dots or commas in there and re-run the code. Exiting.')
-            sys.exit(1)
+            # If no punctuation present, split mid-sentence and throw warning
+            if strict:
+                warnings.warn(f'No punctuation or comma in text - cannot split accordingly. To bypass, re-run the command using strict = False! Exiting. Problematic text: \n\n {text}')
+                sys.exit(1)
+            else: 
+                warnings.warn(f'No punctuation or comma in text - splitting mid-sentence. Problematic text: \n\n {text} \n\n')
+                is_punctuation = [i % split_length == 0 for i in range(1, len(tokens))]
+
     punctuation_indices = [0] + [i for i,v in enumerate(is_punctuation) if v]
 
     # Find intervals that are smaller than the specified split_length
     split_indices = []
     previous_index = 0
     target = split_length
     while target < len(tokens):
         # print('target: ' + str(target))
         checkpoints = [i - target for i in punctuation_indices]
         closest_index = len(list(filter(lambda x: x <= 0, checkpoints))) - 1
-        # print('closest_index: ' + str(closest_index) + ' >> ' + str(punctuation_indices[closest_index]))
-        split_indices.append(punctuation_indices[closest_index])
-        # print('difference at closest_index: ' + str(target - punctuation_indices[closest_index]))
+        # If there is a punctuation gap, larger than split_length
         if closest_index == previous_index:
-            sys.exit('Loop failed. Cannot split the text, since two adjacent punctuations are more than split_length tokens apart. Increase the split_length parameter. ')
-        else:
-            target += split_length - (target - punctuation_indices[closest_index])
-        # print('split_indices: ' + str(split_indices))
+            # If strict, do not split mid-sentence
+            if strict:
+                sys.exit(f'Loop failed. Cannot split the text, since two adjacent punctuations are more than split_length tokens apart. To bypass, re-run the command with strict = False! Problematic text: \n\n {text} \n\n ')
+            # If not strict, insert a new checkpoint mid-sentence and continue
+            else:
+                punctuation_indices.append(punctuation_indices[previous_index] + split_length)
+                punctuation_indices.sort()
+                closest_index += 1
+        target += split_length - (target - punctuation_indices[closest_index])
+
+        split_indices.append(punctuation_indices[closest_index])
         previous_index = closest_index
 
     # Insert split token after punctuation at the computed indices, 
     # then glue the text back together
     offset = 1
     for s in split_indices:
         tokens.insert(s+offset, split_token)
```

### Comparing `secretaries-0.0.1.7/LICENSE` & `secretaries-0.0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `secretaries-0.0.1.7/README.md` & `secretaries-0.0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `secretaries-0.0.1.7/pyproject.toml` & `secretaries-0.0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/secretaries"]
 
 [project]
 name = "secretaries"
-version = "0.0.1.7"
+version = "0.0.1.8"
 license = "MIT"
 authors = [
   { name="Erik Broman", email="mikroberna@gmail.com" },
 ]
 description = "A utility for removing personal data in text."
 readme = "README.md"
 requires-python = ">=3.9"
@@ -30,9 +30,9 @@
             "Operating System :: OS Independent",
             "License :: OSI Approved :: MIT License",
             "Natural Language :: Swedish",
             "Natural Language :: English",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/er1kb/secretary"
-"Bug Tracker" = "https://github.com/er1kb/secretary/issues"
+"Homepage" = "https://github.com/er1kb/secretaries"
+"Bug Tracker" = "https://github.com/er1kb/secretaries/issues"
```

### Comparing `secretaries-0.0.1.7/PKG-INFO` & `secretaries-0.0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: secretaries
-Version: 0.0.1.7
+Version: 0.0.1.8
 Summary: A utility for removing personal data in text.
-Project-URL: Homepage, https://github.com/er1kb/secretary
-Project-URL: Bug Tracker, https://github.com/er1kb/secretary/issues
+Project-URL: Homepage, https://github.com/er1kb/secretaries
+Project-URL: Bug Tracker, https://github.com/er1kb/secretaries/issues
 Author-email: Erik Broman <mikroberna@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: anonymization,gdpr,personal data,personuppgifter,python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
```

