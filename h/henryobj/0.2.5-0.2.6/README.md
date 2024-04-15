# Comparing `tmp/henryobj-0.2.5.tar.gz` & `tmp/henryobj-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henryobj-0.2.5.tar", last modified: Thu Apr 11 13:11:27 2024, max compression
+gzip compressed data, was "henryobj-0.2.6.tar", last modified: Mon Apr 15 10:24:13 2024, max compression
```

## Comparing `henryobj-0.2.5.tar` & `henryobj-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-11 13:11:27.072238 henryobj-0.2.5/
--rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-11 13:11:27.072104 henryobj-0.2.5/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)     2976 2024-01-24 08:03:39.000000 henryobj-0.2.5/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-11 13:11:27.071335 henryobj-0.2.5/henryobj/
--rw-r--r--   0 henry      (501) staff       (20)      224 2024-04-09 07:08:41.000000 henryobj-0.2.5/henryobj/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)    22625 2024-04-11 08:30:24.000000 henryobj-0.2.5/henryobj/base.py
--rw-r--r--   0 henry      (501) staff       (20)     1543 2024-04-10 09:35:13.000000 henryobj-0.2.5/henryobj/config.py
--rw-r--r--   0 henry      (501) staff       (20)    13971 2024-04-11 08:30:55.000000 henryobj-0.2.5/henryobj/gpt.py
--rw-r--r--   0 henry      (501) staff       (20)    29910 2024-04-11 13:11:10.000000 henryobj-0.2.5/henryobj/oai.py
--rw-r--r--   0 henry      (501) staff       (20)    14268 2024-04-11 08:33:40.000000 henryobj-0.2.5/henryobj/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-11 13:11:27.071925 henryobj-0.2.5/henryobj.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-11 13:11:27.000000 henryobj-0.2.5/henryobj.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      282 2024-04-11 13:11:27.000000 henryobj-0.2.5/henryobj.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-04-11 13:11:27.000000 henryobj-0.2.5/henryobj.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       60 2024-04-11 13:11:27.000000 henryobj-0.2.5/henryobj.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)        9 2024-04-11 13:11:27.000000 henryobj-0.2.5/henryobj.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-04-11 13:11:27.072276 henryobj-0.2.5/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      574 2024-04-11 13:11:21.000000 henryobj-0.2.5/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-15 10:24:13.974694 henryobj-0.2.6/
+-rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-15 10:24:13.974515 henryobj-0.2.6/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)     2976 2024-01-24 08:03:39.000000 henryobj-0.2.6/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-15 10:24:13.973530 henryobj-0.2.6/henryobj/
+-rw-r--r--   0 henry      (501) staff       (20)      224 2024-04-09 07:08:41.000000 henryobj-0.2.6/henryobj/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)    22625 2024-04-11 08:30:24.000000 henryobj-0.2.6/henryobj/base.py
+-rw-r--r--   0 henry      (501) staff       (20)     1543 2024-04-10 09:35:13.000000 henryobj-0.2.6/henryobj/config.py
+-rw-r--r--   0 henry      (501) staff       (20)    13971 2024-04-11 08:30:55.000000 henryobj-0.2.6/henryobj/gpt.py
+-rw-r--r--   0 henry      (501) staff       (20)    29910 2024-04-11 13:11:10.000000 henryobj-0.2.6/henryobj/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)    14269 2024-04-15 10:23:49.000000 henryobj-0.2.6/henryobj/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-15 10:24:13.974309 henryobj-0.2.6/henryobj.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-15 10:24:13.000000 henryobj-0.2.6/henryobj.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      282 2024-04-15 10:24:13.000000 henryobj-0.2.6/henryobj.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-04-15 10:24:13.000000 henryobj-0.2.6/henryobj.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       60 2024-04-15 10:24:13.000000 henryobj-0.2.6/henryobj.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)        9 2024-04-15 10:24:13.000000 henryobj-0.2.6/henryobj.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-04-15 10:24:13.974742 henryobj-0.2.6/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      574 2024-04-15 10:24:02.000000 henryobj-0.2.6/setup.py
```

### Comparing `henryobj-0.2.5/PKG-INFO` & `henryobj-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henryobj
-Version: 0.2.5
+Version: 0.2.6
 Home-page: https://github.com/HenryObj/mypip
 Description-Content-Type: text/markdown
 
 # PIP Package henryobj Overview - 24th of January
 
 This codebase is a Python package designed to facilitate web scraping, interactions with OpenAI's API, and provide a suite of utility functions. It is structured to be modular, allowing each component to function independently or in conjunction with others, promoting maintainability and scalability.
```

### Comparing `henryobj-0.2.5/README.md` & `henryobj-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.5/henryobj/base.py` & `henryobj-0.2.6/henryobj/base.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.5/henryobj/config.py` & `henryobj-0.2.6/henryobj/config.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.5/henryobj/gpt.py` & `henryobj-0.2.6/henryobj/gpt.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.5/henryobj/oai.py` & `henryobj-0.2.6/henryobj/oai.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.5/henryobj/web.py` & `henryobj-0.2.6/henryobj/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
         max_words (int, optional): The maximum number of words a sentence can have. Defaults to 50.
 
     Returns:
         str: Text with long sentences removed.
     """
     # Use regex to split text into sentences
     #re.split(r'(?<!\w\.\w.)(?<![A-Z][a-z]\.)(?<=\.|\?)\s', text)
-    sentences = re.split('(?<!\w\.\w.)(?<![A-Z][a-z]\.)(?<=\.|\?)\s', text)
+    sentences = re.split(r'(?<!\w\.\w.)(?<![A-Z][a-z]\.)(?<=\.|\?)\s', text)
     cleaned_sentences = [sentence for sentence in sentences if len(sentence.split()) <= max_words]
     return ' '.join(cleaned_sentences)
 
 def remove_reviews(soup : BeautifulSoup) -> BeautifulSoup:
     """
     Slightly risky function which removes the reviews from a Shopify store.
     """
```

### Comparing `henryobj-0.2.5/henryobj.egg-info/PKG-INFO` & `henryobj-0.2.6/henryobj.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henryobj
-Version: 0.2.5
+Version: 0.2.6
 Home-page: https://github.com/HenryObj/mypip
 Description-Content-Type: text/markdown
 
 # PIP Package henryobj Overview - 24th of January
 
 This codebase is a Python package designed to facilitate web scraping, interactions with OpenAI's API, and provide a suite of utility functions. It is structured to be modular, allowing each component to function independently or in conjunction with others, promoting maintainability and scalability.
```

### Comparing `henryobj-0.2.5/setup.py` & `henryobj-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="henryobj",
-    version="0.2.5", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.2.6", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/mypip',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

