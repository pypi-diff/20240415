# Comparing `tmp/markdown-word-count-0.0.1.tar.gz` & `tmp/markdown_word_count-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/markdown-word-count-0.0.1.tar", last modified: Sun Jul 26 16:26:52 2020, max compression
+gzip compressed data, was "markdown_word_count-0.1.0.tar", last modified: Mon Apr 15 09:32:07 2024, max compression
```

## Comparing `markdown-word-count-0.0.1.tar` & `markdown_word_count-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 gandreadis   (501) staff       (20)        0 2020-07-26 16:26:52.724184 markdown-word-count-0.0.1/
--rw-r--r--   0 gandreadis   (501) staff       (20)     1905 2020-07-26 16:26:52.723824 markdown-word-count-0.0.1/PKG-INFO
--rw-r--r--   0 gandreadis   (501) staff       (20)     1097 2020-07-26 15:48:07.000000 markdown-word-count-0.0.1/README.md
-drwxr-xr-x   0 gandreadis   (501) staff       (20)        0 2020-07-26 16:26:52.721173 markdown-word-count-0.0.1/markdown_word_count.egg-info/
--rw-r--r--   0 gandreadis   (501) staff       (20)     1905 2020-07-26 16:26:52.000000 markdown-word-count-0.0.1/markdown_word_count.egg-info/PKG-INFO
--rw-r--r--   0 gandreadis   (501) staff       (20)      278 2020-07-26 16:26:52.000000 markdown-word-count-0.0.1/markdown_word_count.egg-info/SOURCES.txt
--rw-r--r--   0 gandreadis   (501) staff       (20)        1 2020-07-26 16:26:52.000000 markdown-word-count-0.0.1/markdown_word_count.egg-info/dependency_links.txt
--rw-r--r--   0 gandreadis   (501) staff       (20)       38 2020-07-26 16:26:52.000000 markdown-word-count-0.0.1/markdown_word_count.egg-info/entry_points.txt
--rw-r--r--   0 gandreadis   (501) staff       (20)        4 2020-07-26 16:26:52.000000 markdown-word-count-0.0.1/markdown_word_count.egg-info/top_level.txt
-drwxr-xr-x   0 gandreadis   (501) staff       (20)        0 2020-07-26 16:26:52.722934 markdown-word-count-0.0.1/mwc/
--rw-r--r--   0 gandreadis   (501) staff       (20)        0 2020-07-26 12:19:34.000000 markdown-word-count-0.0.1/mwc/__init__.py
--rwxr-xr-x   0 gandreadis   (501) staff       (20)      717 2020-07-26 12:44:03.000000 markdown-word-count-0.0.1/mwc/cli.py
--rw-r--r--   0 gandreadis   (501) staff       (20)     1023 2020-07-26 12:44:03.000000 markdown-word-count-0.0.1/mwc/counter.py
--rw-r--r--   0 gandreadis   (501) staff       (20)       38 2020-07-26 16:26:52.724317 markdown-word-count-0.0.1/setup.cfg
--rw-r--r--   0 gandreadis   (501) staff       (20)      733 2020-07-26 16:26:34.000000 markdown-word-count-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:32:07.290526 markdown_word_count-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-15 09:32:03.000000 markdown_word_count-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-15 09:32:07.290526 markdown_word_count-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-15 09:32:03.000000 markdown_word_count-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:32:07.290526 markdown_word_count-0.1.0/markdown_word_count.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-15 09:32:07.000000 markdown_word_count-0.1.0/markdown_word_count.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-15 09:32:07.000000 markdown_word_count-0.1.0/markdown_word_count.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:32:07.000000 markdown_word_count-0.1.0/markdown_word_count.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 09:32:07.000000 markdown_word_count-0.1.0/markdown_word_count.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 09:32:07.000000 markdown_word_count-0.1.0/markdown_word_count.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:32:07.290526 markdown_word_count-0.1.0/mwc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:32:03.000000 markdown_word_count-0.1.0/mwc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-04-15 09:32:03.000000 markdown_word_count-0.1.0/mwc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-15 09:32:03.000000 markdown_word_count-0.1.0/mwc/counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:32:07.290526 markdown_word_count-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-15 09:32:03.000000 markdown_word_count-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:32:07.290526 markdown_word_count-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-15 09:32:03.000000 markdown_word_count-0.1.0/tests/test_mwc.py
```

### Comparing `markdown-word-count-0.0.1/README.md` & `markdown_word_count-0.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,57 @@
 # ⬇ Markdown Word Count
 
-[![CircleCI status](https://circleci.com/gh/gandreadis/markdown-word-count.svg?style=svg)](https://circleci.com/gh/gandreadis/markdown-word-count)
+[![Python package](https://github.com/gandreadis/markdown-word-count/actions/workflows/python-package.yml/badge.svg)](https://github.com/gandreadis/markdown-word-count/actions/workflows/python-package.yml)
 
 A word counter for raw Markdown files, excluding punctuation, footnotes, and special Markdown or HTML tag syntax.
 
 ## 💻 Installation
 
 You will need...
 
 - 🐍 Python 3
-- 🐑 A [clone](https://github.com/gandreadis/markdown-word-count.git) of this repo or a [single file download](https://github.com/gandreadis/markdown-word-count/blob/master/mwc.py) of the script.
+- 🐑 PIP3 or a [clone](https://github.com/gandreadis/markdown-word-count.git) of this repo.
 
 ## ▶ Usage
 
-To run this script, pass the file you want to have analyzed as the first parameter:
+### Through PIP
+
+The easiest way is to run:
+
+```
+pip install markdown-word-count
+```
+
+Then, you'll be able to analyze any file by passing its name (relative path) to the `mwc` script:
 
 ```
-./mwc.py myfile.md
+mwc yourfile.md
 ```
 
-If that doesn't work, explicitly pass the program to Python:
+You can also pass in multiple files or a blob if your shell supports it. This allows for checking all files in a folder, for example.
+
+```
+mwc text1.md text2.md
+mwc test/*.md
+```
+
+### Manually
+
+If you want to clone the repo and run the Python script manually, run:
 
 ```
-python mwc.py myfile.md
+python mwc/cli.py myfile.md
 ```
 
 If this doesn't work, try `python3` instead of `python`.
 
 ## ⛏ Development
 
 Run this to execute all tests:
 
 ```
 python -m unittest discover
 ```
 
 ## 💬 Ports to Other Programming Languages
 
-* A PHP port can be found [here](https://github.com/Arcesilas/md-word-count), with thanks to [@Arcesilas](https://github.com/Arcesilas)!
+- A PHP port can be found [here](https://github.com/Arcesilas/md-word-count), with thanks to [@Arcesilas](https://github.com/Arcesilas)!
```

### Comparing `markdown-word-count-0.0.1/mwc/cli.py` & `markdown_word_count-0.1.0/mwc/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,27 +2,46 @@
 # -*- coding: utf-8 -*-
 import os
 import sys
 
 from mwc.counter import count_words_in_markdown
 
 
+def get_count(files):
+    count = 0
+    for file in files:
+        if not os.path.isfile(file):
+            print('The file at the given location {file} could not be opened')
+            sys.exit(1)
+        with open(file, 'r', encoding='utf8') as f:
+            count += count_words_in_markdown(f.read())
+
+    return count
+
+
 def main():
     if sys.version_info < (3,):
-        print('Python 3 is required. You are using Python 2. You should probably run this script as follows:')
+        print(
+            'Python 3 is required. You are using Python 2. You should probably run this script as follows:')
         print('python3 mwc.py')
         sys.exit(1)
 
     if len(sys.argv) < 2:
         print('Provide the Markdown file to parse as first argument')
         sys.exit(1)
 
-    if not os.path.isfile(sys.argv[1]):
-        print('The file at the given location could not be opened')
-        sys.exit(1)
+    files = sys.argv[1:]
+
+    count = get_count(files)
+
+    if len(files) == 1:
+        print(f"Number of words in file {files[0]}")
+        print(count)
+    else:
+        print(f"Words across {len(files)} files")
+        print(count)
 
-    with open(sys.argv[1], 'r', encoding='utf8') as f:
-        print(count_words_in_markdown(f.read()))
+    return count
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `markdown-word-count-0.0.1/mwc/counter.py` & `markdown_word_count-0.1.0/mwc/counter.py`

 * *Files identical despite different names*

### Comparing `markdown-word-count-0.0.1/setup.py` & `markdown_word_count-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="markdown-word-count",
-    version="0.0.1",
+    version="0.1.0",
     author="Georgios Andreadis",
     author_email="info@gandreadis.com",
     description="Word counter for raw Markdown files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gandreadis/markdown-word-count",
     packages=['mwc'],
```

