# Comparing `tmp/langbank-0.1.tar.gz` & `tmp/langbank-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langbank-0.1.tar", last modified: Sun Apr 14 17:45:26 2024, max compression
+gzip compressed data, was "langbank-0.1.2.tar", last modified: Mon Apr 15 10:38:49 2024, max compression
```

## Comparing `langbank-0.1.tar` & `langbank-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-14 17:45:26.477219 langbank-0.1/
--rw-r--r--   0 teddygonyea   (501) staff       (20)       50 2024-04-14 17:45:26.477026 langbank-0.1/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)        0 2024-04-13 23:34:58.000000 langbank-0.1/README.md
--rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-14 17:45:26.477281 langbank-0.1/setup.cfg
--rw-r--r--   0 teddygonyea   (501) staff       (20)      164 2024-04-14 12:26:14.000000 langbank-0.1/setup.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-14 17:45:26.475352 langbank-0.1/src/
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-14 17:45:26.475884 langbank-0.1/src/langbank/
--rw-r--r--   0 teddygonyea   (501) staff       (20)       27 2024-04-14 12:25:24.000000 langbank-0.1/src/langbank/__init__.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     3268 2024-04-14 17:42:04.000000 langbank-0.1/src/langbank/main.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-14 17:45:26.476810 langbank-0.1/src/langbank.egg-info/
--rw-r--r--   0 teddygonyea   (501) staff       (20)       50 2024-04-14 17:45:26.000000 langbank-0.1/src/langbank.egg-info/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)      208 2024-04-14 17:45:26.000000 langbank-0.1/src/langbank.egg-info/SOURCES.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-14 17:45:26.000000 langbank-0.1/src/langbank.egg-info/dependency_links.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)        9 2024-04-14 17:45:26.000000 langbank-0.1/src/langbank.egg-info/top_level.txt
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:38:49.522431 langbank-0.1.2/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     1304 2024-04-15 10:38:49.522178 langbank-0.1.2/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     1032 2024-04-15 09:49:18.000000 langbank-0.1.2/README.md
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-15 10:38:49.522469 langbank-0.1.2/setup.cfg
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      492 2024-04-15 10:38:43.000000 langbank-0.1.2/setup.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:38:49.520524 langbank-0.1.2/src/
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:38:49.521153 langbank-0.1.2/src/langbank/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       27 2024-04-14 12:25:24.000000 langbank-0.1.2/src/langbank/__init__.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     4429 2024-04-15 10:15:02.000000 langbank-0.1.2/src/langbank/main.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:38:49.521991 langbank-0.1.2/src/langbank.egg-info/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     1304 2024-04-15 10:38:49.000000 langbank-0.1.2/src/langbank.egg-info/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      208 2024-04-15 10:38:49.000000 langbank-0.1.2/src/langbank.egg-info/SOURCES.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-15 10:38:49.000000 langbank-0.1.2/src/langbank.egg-info/dependency_links.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)        9 2024-04-15 10:38:49.000000 langbank-0.1.2/src/langbank.egg-info/top_level.txt
```

### Comparing `langbank-0.1/src/langbank/main.py` & `langbank-0.1.2/src/langbank/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,20 +17,36 @@
         """
         if file_path is None:
             # Default file path: ~/langbank/bank.json
             self.file_path = os.path.expanduser("~/langbank/bank.json")
         else:
             self.file_path = file_path
 
+        self.setup_bank()
+
     def set_file_path(self, file_path):
         """
         Set the file path for the word bank.
         """
         self.file_path = file_path
 
+    def setup_bank(self):
+        """
+        Create the word bank file and parent directories if they do not exist.
+        """
+        # Create parent directories if they do not exist
+        parent_dir = os.path.dirname(self.file_path)
+        if not os.path.exists(parent_dir):
+            os.makedirs(parent_dir)
+
+        # Create the word bank file if it does not exist
+        if not os.path.exists(self.file_path):
+            with open(self.file_path, "w") as f:
+                f.write("[]")
+
     def get_bank(self):
         """
         Get the contents of the word bank from the JSON file.
         Returns:
             The word bank (list).
         Raises:
             FileNotFoundError: If the file does not exist.
@@ -70,19 +86,17 @@
             word: the word to add
             tags: a list of string tags
         """
         if tags is None:
             tags = []
 
         dt = datetime.now()
-        entry = {"word": word, "datetime": dt, "tags": tags}
-        bank = self.get_bank()
-        bank.append(entry)
-
-        self.write_bank(bank)
+        entry = {"word": word, "datetime": dt.strftime(DATETIME_FORMAT), "tags": tags}
+        with open(self.file_path, "a") as f:
+            f.write(json.dumps(entry) + "\n")
 
     def get_words_from_past_n_days(self, n=0):
         """
         Get a list of all the words added in the past n days, where n=0 will return the words added today
         """
         bank = self.get_bank()
         today = datetime.now().date()
@@ -106,7 +120,31 @@
         bank = self.get_bank()
         words = []
         for entry in bank:
             if tag in entry["tags"]:
                 words.append(entry["word"])
 
         return words
+
+    def get_words_by_date(self, date):
+        """
+        Get a list of all the words added on a specific date
+        """
+        bank = self.get_bank()
+        words = []
+        for entry in bank:
+            if entry["datetime"].date() == date:
+                words.append(entry["word"])
+
+        return words
+
+    def occurences(self, word):
+        """
+        Get the number of times a word has been added to the bank
+        """
+        bank = self.get_bank()
+        count = 0
+        for entry in bank:
+            if entry["word"] == word:
+                count += 1
+
+        return count
```

