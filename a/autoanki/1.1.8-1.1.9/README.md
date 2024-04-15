# Comparing `tmp/autoanki-1.1.8.tar.gz` & `tmp/autoanki-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoanki-1.1.8.tar", last modified: Thu Apr 11 22:10:28 2024, max compression
+gzip compressed data, was "autoanki-1.1.9.tar", last modified: Mon Apr 15 21:47:26 2024, max compression
```

## Comparing `autoanki-1.1.8.tar` & `autoanki-1.1.9.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.992928 autoanki-1.1.8/
--rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.1.8/LICENSE.txt
--rw-r--r--   0 owner      (501) staff       (20)       75 2023-05-05 18:09:43.000000 autoanki-1.1.8/MANIFEST.in
--rw-r--r--   0 owner      (501) staff       (20)     5008 2024-04-11 22:10:28.992849 autoanki-1.1.8/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)     4475 2024-04-10 21:23:08.000000 autoanki-1.1.8/README.md
--rw-r--r--   0 owner      (501) staff       (20)      223 2023-05-05 21:35:51.000000 autoanki-1.1.8/pyproject.toml
--rw-r--r--   0 owner      (501) staff       (20)      699 2024-04-11 22:10:28.993223 autoanki-1.1.8/setup.cfg
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.984964 autoanki-1.1.8/src/
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.986823 autoanki-1.1.8/src/autoanki/
--rw-r--r--   0 owner      (501) staff       (20)    10590 2024-04-10 20:36:12.000000 autoanki-1.1.8/src/autoanki/AutoAnki.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.988498 autoanki-1.1.8/src/autoanki/BookCleaner/
--rw-r--r--   0 owner      (501) staff       (20)     7455 2024-04-10 20:32:34.000000 autoanki-1.1.8/src/autoanki/BookCleaner/BookCleaner.py
--rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.1.8/src/autoanki/BookCleaner/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.989820 autoanki-1.1.8/src/autoanki/DatabaseManager/
--rw-r--r--   0 owner      (501) staff       (20)    15691 2024-04-11 21:45:12.000000 autoanki-1.1.8/src/autoanki/DatabaseManager/DatabaseManager.py
--rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.1.8/src/autoanki/DatabaseManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.1.8/src/autoanki/DatabaseManager/book_table.sql
--rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.1.8/src/autoanki/DatabaseManager/book_table_view.sql
--rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.1.8/src/autoanki/DatabaseManager/databases_init.sql
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.990916 autoanki-1.1.8/src/autoanki/DeckManager/
--rw-r--r--   0 owner      (501) staff       (20)     4210 2024-04-08 21:24:06.000000 autoanki-1.1.8/src/autoanki/DeckManager/DeckManager.py
--rw-r--r--   0 owner      (501) staff       (20)       67 2024-04-04 22:41:18.000000 autoanki-1.1.8/src/autoanki/DeckManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)     2676 2024-04-06 21:14:34.000000 autoanki-1.1.8/src/autoanki/DeckManager/template_decks.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.992149 autoanki-1.1.8/src/autoanki/Dictionary/
--rw-r--r--   0 owner      (501) staff       (20)     4627 2024-04-11 22:10:15.000000 autoanki-1.1.8/src/autoanki/Dictionary/CEDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)      286 2024-04-05 16:04:00.000000 autoanki-1.1.8/src/autoanki/Dictionary/Dictionary.py
--rw-r--r--   0 owner      (501) staff       (20)     5320 2024-04-07 04:26:04.000000 autoanki-1.1.8/src/autoanki/Dictionary/YellowBridgeDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)       40 2024-03-31 20:26:56.000000 autoanki-1.1.8/src/autoanki/Dictionary/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.1.8/src/autoanki/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-11 22:10:28.992569 autoanki-1.1.8/src/autoanki.egg-info/
--rw-r--r--   0 owner      (501) staff       (20)     5008 2024-04-11 22:10:28.000000 autoanki-1.1.8/src/autoanki.egg-info/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)      878 2024-04-11 22:10:28.000000 autoanki-1.1.8/src/autoanki.egg-info/SOURCES.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2024-04-11 22:10:28.000000 autoanki-1.1.8/src/autoanki.egg-info/dependency_links.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.1.8/src/autoanki.egg-info/not-zip-safe
--rw-r--r--   0 owner      (501) staff       (20)        9 2024-04-11 22:10:28.000000 autoanki-1.1.8/src/autoanki.egg-info/top_level.txt
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.161110 autoanki-1.1.9/
+-rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.1.9/LICENSE.txt
+-rw-r--r--   0 owner      (501) staff       (20)      110 2024-04-15 18:10:25.000000 autoanki-1.1.9/MANIFEST.in
+-rw-r--r--   0 owner      (501) staff       (20)     5558 2024-04-15 21:47:26.161024 autoanki-1.1.9/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)     5024 2024-04-15 21:45:41.000000 autoanki-1.1.9/README.md
+-rw-r--r--   0 owner      (501) staff       (20)      223 2023-05-05 21:35:51.000000 autoanki-1.1.9/pyproject.toml
+-rw-r--r--   0 owner      (501) staff       (20)      700 2024-04-15 21:47:26.162032 autoanki-1.1.9/setup.cfg
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.138400 autoanki-1.1.9/src/
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.140272 autoanki-1.1.9/src/autoanki/
+-rw-r--r--   0 owner      (501) staff       (20)     6228 2024-04-15 21:29:46.000000 autoanki-1.1.9/src/autoanki/AutoAnki.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.141950 autoanki-1.1.9/src/autoanki/BookCleaner/
+-rw-r--r--   0 owner      (501) staff       (20)     4435 2024-04-15 18:04:41.000000 autoanki-1.1.9/src/autoanki/BookCleaner/BookCleaner.py
+-rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.1.9/src/autoanki/BookCleaner/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.143228 autoanki-1.1.9/src/autoanki/DatabaseManager/
+-rw-r--r--   0 owner      (501) staff       (20)    13775 2024-04-15 20:45:52.000000 autoanki-1.1.9/src/autoanki/DatabaseManager/DatabaseManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.1.9/src/autoanki/DatabaseManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.1.9/src/autoanki/DatabaseManager/book_table.sql
+-rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.1.9/src/autoanki/DatabaseManager/book_table_view.sql
+-rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.1.9/src/autoanki/DatabaseManager/databases_init.sql
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.144090 autoanki-1.1.9/src/autoanki/DeckManager/
+-rw-r--r--   0 owner      (501) staff       (20)     4692 2024-04-15 21:30:15.000000 autoanki-1.1.9/src/autoanki/DeckManager/DeckManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       67 2024-04-04 22:41:18.000000 autoanki-1.1.9/src/autoanki/DeckManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)     2654 2024-04-15 21:12:02.000000 autoanki-1.1.9/src/autoanki/DeckManager/template_decks.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.145512 autoanki-1.1.9/src/autoanki/Dictionary/
+-rw-r--r--   0 owner      (501) staff       (20)     5791 2024-04-15 21:07:12.000000 autoanki-1.1.9/src/autoanki/Dictionary/CEDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)      286 2024-04-12 01:17:18.000000 autoanki-1.1.9/src/autoanki/Dictionary/Dictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)     5339 2024-04-15 18:03:31.000000 autoanki-1.1.9/src/autoanki/Dictionary/YellowBridgeDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)       40 2024-03-31 20:26:56.000000 autoanki-1.1.9/src/autoanki/Dictionary/__init__.py
+-rw-rw-r--   0 owner      (501) staff       (20)  9650508 2024-04-10 22:45:58.000000 autoanki-1.1.9/src/autoanki/Dictionary/cedict_ts.u8
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.158726 autoanki-1.1.9/src/autoanki/Tokenizer/
+-rw-r--r--   0 owner      (501) staff       (20)     6607 2024-04-15 21:23:30.000000 autoanki-1.1.9/src/autoanki/Tokenizer/ChineseTokenizer.py
+-rw-r--r--   0 owner      (501) staff       (20)      223 2024-04-12 14:29:21.000000 autoanki-1.1.9/src/autoanki/Tokenizer/Tokenizer.py
+-rw-r--r--   0 owner      (501) staff       (20)       48 2024-04-11 22:24:23.000000 autoanki-1.1.9/src/autoanki/Tokenizer/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.1.9/src/autoanki/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.160659 autoanki-1.1.9/src/autoanki.egg-info/
+-rw-r--r--   0 owner      (501) staff       (20)     5558 2024-04-15 21:47:26.000000 autoanki-1.1.9/src/autoanki.egg-info/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)     1029 2024-04-15 21:47:26.000000 autoanki-1.1.9/src/autoanki.egg-info/SOURCES.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2024-04-15 21:47:26.000000 autoanki-1.1.9/src/autoanki.egg-info/dependency_links.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.1.9/src/autoanki.egg-info/not-zip-safe
+-rw-r--r--   0 owner      (501) staff       (20)        9 2024-04-15 21:47:26.000000 autoanki-1.1.9/src/autoanki.egg-info/top_level.txt
```

### Comparing `autoanki-1.1.8/LICENSE.txt` & `autoanki-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.8/PKG-INFO` & `autoanki-1.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.1.8
+Version: 1.1.9
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 > **❗️** <br>
 Pull requests welcome! If you think you can improve AA in any way, open a PR!
 
 # autoanki
@@ -64,14 +64,28 @@
 Import this file into Anki, and you're all set.
 
 #### Other commands
 If you want to see the status of the database, use:
 ```
 aa.print_database_info()
 ```
+If you would like to create and use your own dictionary, you can pass it in when you 
+```
+aa = AutoAnki(db_path, dictionary=CustomDictionary())
+```
+This dictionary must implement functions from the abstract class `autoanki/Dictionary.py`
+
+Some settings can be set regarding how cards will be formatted, and what will be shown. They can be seen here:
+```
+aa.deck_settings(
+include_traditional=True,
+include_part_of_speech=True,
+word_frequency_filter=1e-05 # Float between 0 and 1. Filters using this library: https://pypi.org/project/wordfreq/
+)
+```
 
 ## How it works
 AutoAnki interfaces has 4 components on the back end:
 1. BookCleaner: Cleans the input coming in from files that the user supplies 
 2. DatabaseManager: Takes the cleaned input and puts it into the database
 3. Dictionary: Finds definitions for words in the database
 4. DeckManager: Creates Decks
```

### Comparing `autoanki-1.1.8/README.md` & `autoanki-1.1.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -49,14 +49,28 @@
 Import this file into Anki, and you're all set.
 
 #### Other commands
 If you want to see the status of the database, use:
 ```
 aa.print_database_info()
 ```
+If you would like to create and use your own dictionary, you can pass it in when you 
+```
+aa = AutoAnki(db_path, dictionary=CustomDictionary())
+```
+This dictionary must implement functions from the abstract class `autoanki/Dictionary.py`
+
+Some settings can be set regarding how cards will be formatted, and what will be shown. They can be seen here:
+```
+aa.deck_settings(
+include_traditional=True,
+include_part_of_speech=True,
+word_frequency_filter=1e-05 # Float between 0 and 1. Filters using this library: https://pypi.org/project/wordfreq/
+)
+```
 
 ## How it works
 AutoAnki interfaces has 4 components on the back end:
 1. BookCleaner: Cleans the input coming in from files that the user supplies 
 2. DatabaseManager: Takes the cleaned input and puts it into the database
 3. Dictionary: Finds definitions for words in the database
 4. DeckManager: Creates Decks
```

### Comparing `autoanki-1.1.8/setup.cfg` & `autoanki-1.1.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = autoanki
-version = 1.1.8
+version = 1.1.9
 author = Jarvis Coghlin
 author_email = jarviscoghlin@gmail.com
 description = Automatically make Anki Decks for Chinese text
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/timmy6figures/autoanki
 project_urls = 
@@ -16,15 +16,15 @@
 
 [options]
 include_package_data = True
 zip_safe = False
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.10
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `autoanki-1.1.8/src/autoanki/DatabaseManager/DatabaseManager.py` & `autoanki-1.1.9/src/autoanki/DatabaseManager/DatabaseManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 import os
-from string import punctuation
 import re
 import sqlite3
 import logging
 import unicodedata
-from glob import glob
 
+from glob import glob
 from pathlib import Path
-import jieba
-import chinese_converter
 
 from autoanki.BookCleaner.BookCleaner import CLEANED_FILES_DIRECTORY
+from autoanki.Tokenizer.ChineseTokenizer import ChineseTokenizer
 
-CHINESE_PUNC = "ｗ９ｌｉｔｂｎｅｐ ！？◇｡。．ｈ＂＃＄％＆＇（）＊＋，－／：；＜＝＞＠［＼］＾＿｀｛｜｝～｟｠｢｣､、〃《》「」『』【】〔〕〖〗〘〙〚〛〜〝〞〟〰〾〿–—‘’‛“”„‟…‧﹏."
-PUNC = "™∞•◎ ♦⑽]■①"
-CHINESE_NUMBERS = "第一二两三四五六七八九十百千万满"
 
 class DatabaseManager:
 
     def __init__(self, database_path, debug_level):
+        # TODO Documentation
         self.logger = logging.getLogger('autoanki.dbmngr')
         self.logger.setLevel(debug_level)
+
+        # Init database
         if not os.path.exists(database_path):
             self.logger.warning("The database [", database_path, "] does not exist.")
             raise Exception("Cannot create DatabaseManager with invalid database path.")
         self.database_path = database_path
-        self.books = []
+
+        # Text segmenter
+        self.tokenizer = ChineseTokenizer(debug_level)
+
+        # Sql connection
         path = os.path.join(os.getcwd(), self.database_path)
         self.connection = sqlite3.connect(path)
         self.cursor = self.connection.cursor()
 
+        self.books = []
+
     @staticmethod
-    def convert_to_tablename(name: str):
+    def convert_to_tablename(name: str) -> str:
         """
         Converts a string to a sql-valid table name.
         `param name` The name to convert
         `return` A tablename valid for an sql table
         """
         value = unicodedata.normalize('NFKC', name)
         # value.replace("：",":")
@@ -113,72 +117,30 @@
         """
         Adds every word in a file to both the dictionary table and the book's table
         `filepath` The path to the file
         `table_name` The name of the table to add the words to.
             This should be the same for every wile in a given book
         """
         self.logger.info(f"Adding [{filepath}] to database...")
-
         word_appearances = {}
         with open(filepath,'r',encoding='utf-8') as f:
             line = " "
             while line:
-                line = f.readline()
+                line = f.readline().strip(" ")
                 if not line:
                     continue
-                words = jieba.lcut(line)
+                words = self.tokenizer.tokenize(line)
+                if not words:
+                    continue
                 for word in words:
-
-                    # TODO There is a lot of shenanigans happening in this section. 
-                    #   This should be split into a Chinese-spesific file, and 
-                    #   some of these rules should be re-evaluated
-                    word = word.lstrip("第")
-                    word = word.lstrip("几")
-
-                    # Repeated characters (always?) contain the same meaning as one, just varied slightly
-                    # 人人 = everyone
-                    if len(word) == 2 and word[0] == word[1]:
-                        word = word[0]
-
-                    # Some gramatical patterns:
-                    if len(word) > 2 and word[0] == "在" and word[-1] == "上":
-                        word = word[1:-2]
-
-
-                    # Remove all numbers from the front
-                    # Lots of the words follow the following format:
-                    #   Number + Subject
-                    old_word = "" 
-                    while old_word != word:
-                        old_word = word
-                        if len(word) == 0:
-                            break
-                        if word[0] in CHINESE_NUMBERS:
-                            word = word[1:]
-
-                    # Remove puncuation
-                    word = word.translate(str.maketrans('', '', punctuation))
-
-                    is_ascii = len(word) == len(word.encode())
-
-                    is_ascii_special = False
-                    if len(word) == 1:
-                        is_ascii_special = ord(word[0]) > 128 and ord(word[0]) < 255 
-
-                    if word in PUNC or word in CHINESE_PUNC or is_ascii or is_ascii_special or word is None:
-                        continue
                     if word_appearances.get(word) == None:
-                        # Convert the word to simplified if needed
-                        word = chinese_converter.to_simplified(word)
                         word_appearances[word] = 1
                     else:
                         word_appearances[word] += 1
 
-
-
         # Add the words to the dictionary if they are not already there
         self.cursor.execute(f"SELECT word FROM dictionary")
         self.connection.commit()
         dictionary_words = self.cursor.fetchall()
         self.logger.info(f"{len(word_appearances.items())} words in file. {len(dictionary_words)} in dictionary.")
 
         for word, appearances in word_appearances.items():
@@ -224,15 +186,14 @@
 
         # self.logger.debug("Done adding file to database")
 
     def insert_word(self, word):
         # TODO Doing this breaks the `number_of_appearances`. This is a temporary fix
         self.cursor.execute("SELECT word FROM dictionary WHERE word = ?", [word])
         all_rows = self.cursor.fetchall()
-        
         if len(all_rows) == 0:
             # self.logger.info("  Inserting")
             self.cursor.execute(f"INSERT INTO dictionary (word) VALUES (?)", [word])
             self.connection.commit()
 
     def remove_word(self, word:str):
         if '*' in word:
@@ -313,29 +274,31 @@
         word_type = params[1]\n
         pinyin = params[2]\n
         pinyin_numbers = params[3]\n
         sub_components = params[4]\n
         hsk_level = params[5]\n
         top_level = params[6]\n
         definition = params[7]\n
-        word = params[8]
+        frequency = params[8]
+        word = params[9]
         :param params: A list of params for the database:
         :return:
         """
         # TODO Some sanatization here might be a good idea
         #   Make sure junk data can't crash this function
         self.cursor.execute("UPDATE dictionary "
                             "SET word_traditional = ?, "
                             "word_type = ?,"
                             "pinyin = ?, "
                             "pinyin_numbers = ?,"
                             "sub_components = ?,"
                             "hsk_level = ?,"
                             "top_level = ?,"
-                            "definition = ?"
+                            "definition = ?,"
+                            "frequency = ?"
                             "WHERE word = ?",
                             params)
         self.connection.commit()
 
     def get_all_completed_definitions(self):
 
         self.cursor.execute("SELECT * FROM dictionary WHERE definition IS NOT NULL")
```

### Comparing `autoanki-1.1.8/src/autoanki/DatabaseManager/databases_init.sql` & `autoanki-1.1.9/src/autoanki/DatabaseManager/databases_init.sql`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.8/src/autoanki/DeckManager/DeckManager.py` & `autoanki-1.1.9/src/autoanki/DeckManager/DeckManager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 
 import genanki
-from genanki import Model
-from pprint import pprint
+from wordfreq import word_frequency
 
-from ..DeckManager import template_decks
+from autoanki.DeckManager import template_decks
 
 class DeckManager:
     """
     The class to make anki decks. Create the file using generate_deck_file()
     One of the most important concepts is the id. No matter what deck the word is in, it should have the same id so the
     same card in different decks can be remembered.
     This class makes extensive use of genanki, so understanding how genanki works
@@ -30,21 +29,23 @@
         self.include_traditional = include_traditional 
         self.include_part_of_speech = include_part_of_speech
 
         self.book_list = []
 
     def settings(self,
                  include_traditional,
-                 include_part_of_speech
+                 include_part_of_speech,
+                 word_frequency_filter
                  ):
         """
         Configures settings for what's in the deck, and how it looks
         """
         self.include_traditional = include_traditional
         self.include_part_of_speech = include_part_of_speech 
+        self.word_frequency_filter = word_frequency_filter 
 
     def generate_deck_file(self, words, deck_name: str, filename: str):
         """
         Generates a deck file from the database
         :param deck_name: The name of the deck to be created
         :param definitions_filename: The name of the file containing the definitions.
         :return:
@@ -57,25 +58,37 @@
         # self.deck.add_note()
         self.deck = genanki.Deck(
             2020000110,
             deck_name
         )
 
         for row in words:
+
+            if self.word_frequency_filter:
+                if self.word_frequency_filter < row['frequency']:
+                    continue
+
             word = row["word"]
 
             if self.include_traditional:
                 word_traditional = row["word_traditional"]
             else:
                 word_traditional = ""
 
             if len(word) != len(word_traditional):
                 self.logger.error(f"{word} and {word_traditional} should be the same length")
-            if word_traditional == word:
-                word_traditional = "-"*len(word)
+
+            # Replace all matching characters with a dash 
+            formatted_word_traditional = ""
+            for i in range(len(word)):
+                if word[i] == word_traditional[i]:
+                    formatted_word_traditional += "-"
+                else:
+                    formatted_word_traditional += word_traditional[i]
+
             if row["pinyin"]:
                 pinyin = row["pinyin"]
             else:
                 pinyin = row["pinyin_numbers"]
             definition = "<br>" + row["definition"]
             # word["word_id"]
             # word["word"]
```

### Comparing `autoanki-1.1.8/src/autoanki/DeckManager/template_decks.py` & `autoanki-1.1.9/src/autoanki/DeckManager/template_decks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import genanki
 from genanki import Model
 
 CHINESE_CARD_MODEL = Model(
     1559383145,
-    'Chinese Card (autoanki)',
+    'autoanki-chinese',
     fields=[
         {
             'name': 'word',
             'font': 'Arial',
         },
         {
             'name': 'word_traditional',
```

### Comparing `autoanki-1.1.8/src/autoanki/Dictionary/YellowBridgeDictionary.py` & `autoanki-1.1.9/src/autoanki/Dictionary/YellowBridgeDictionary.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import requests
 import selenium
 from selenium import webdriver
 from bs4 import BeautifulSoup
 import urllib.parse
 import pinyin as pin_to_num
 
-from .Dictionary import Dictionary
+from autoanki.Dictionary.Dictionary import Dictionary
 
 class YellowBridgeDictionary(Dictionary):
 
     def __init__(self, debug_level):
         self.logger = logging.getLogger('autoanki.ybdict')
         self.logger.setLevel(debug_level)
         self.logger.debug(f"logger active")
```

### Comparing `autoanki-1.1.8/src/autoanki.egg-info/PKG-INFO` & `autoanki-1.1.9/src/autoanki.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.1.8
+Version: 1.1.9
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 > **❗️** <br>
 Pull requests welcome! If you think you can improve AA in any way, open a PR!
 
 # autoanki
@@ -64,14 +64,28 @@
 Import this file into Anki, and you're all set.
 
 #### Other commands
 If you want to see the status of the database, use:
 ```
 aa.print_database_info()
 ```
+If you would like to create and use your own dictionary, you can pass it in when you 
+```
+aa = AutoAnki(db_path, dictionary=CustomDictionary())
+```
+This dictionary must implement functions from the abstract class `autoanki/Dictionary.py`
+
+Some settings can be set regarding how cards will be formatted, and what will be shown. They can be seen here:
+```
+aa.deck_settings(
+include_traditional=True,
+include_part_of_speech=True,
+word_frequency_filter=1e-05 # Float between 0 and 1. Filters using this library: https://pypi.org/project/wordfreq/
+)
+```
 
 ## How it works
 AutoAnki interfaces has 4 components on the back end:
 1. BookCleaner: Cleans the input coming in from files that the user supplies 
 2. DatabaseManager: Takes the cleaned input and puts it into the database
 3. Dictionary: Finds definitions for words in the database
 4. DeckManager: Creates Decks
```

### Comparing `autoanki-1.1.8/src/autoanki.egg-info/SOURCES.txt` & `autoanki-1.1.9/src/autoanki.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,8 +19,12 @@
 src/autoanki/DatabaseManager/databases_init.sql
 src/autoanki/DeckManager/DeckManager.py
 src/autoanki/DeckManager/__init__.py
 src/autoanki/DeckManager/template_decks.py
 src/autoanki/Dictionary/CEDictionary.py
 src/autoanki/Dictionary/Dictionary.py
 src/autoanki/Dictionary/YellowBridgeDictionary.py
-src/autoanki/Dictionary/__init__.py
+src/autoanki/Dictionary/__init__.py
+src/autoanki/Dictionary/cedict_ts.u8
+src/autoanki/Tokenizer/ChineseTokenizer.py
+src/autoanki/Tokenizer/Tokenizer.py
+src/autoanki/Tokenizer/__init__.py
```

