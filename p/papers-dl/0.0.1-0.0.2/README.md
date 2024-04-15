# Comparing `tmp/papers_dl-0.0.1.tar.gz` & `tmp/papers_dl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papers_dl-0.0.1.tar", last modified: Sun Apr 14 23:02:16 2024, max compression
+gzip compressed data, was "papers_dl-0.0.2.tar", last modified: Mon Apr 15 18:11:45 2024, max compression
```

## Comparing `papers_dl-0.0.1.tar` & `papers_dl-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-14 23:02:16.780367 papers_dl-0.0.1/
--rw-r--r--   0 ben        (501) staff       (20)     1070 2024-03-23 22:45:07.000000 papers_dl-0.0.1/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)     1299 2024-04-14 23:02:16.780105 papers_dl-0.0.1/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      766 2024-04-14 00:32:36.000000 papers_dl-0.0.1/README.md
--rw-r--r--   0 ben        (501) staff       (20)      603 2024-04-14 23:02:09.000000 papers_dl-0.0.1/pyproject.toml
--rw-r--r--   0 ben        (501) staff       (20)       38 2024-04-14 23:02:16.780413 papers_dl-0.0.1/setup.cfg
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-14 23:02:16.778146 papers_dl-0.0.1/src/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-14 23:02:16.779708 papers_dl-0.0.1/src/papers_dl.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     1299 2024-04-14 23:02:16.000000 papers_dl-0.0.1/src/papers_dl.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      208 2024-04-14 23:02:16.000000 papers_dl-0.0.1/src/papers_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2024-04-14 23:02:16.000000 papers_dl-0.0.1/src/papers_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)        7 2024-04-14 23:02:16.000000 papers_dl-0.0.1/src/papers_dl.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)    10431 2024-04-14 01:36:31.000000 papers_dl-0.0.1/src/scihub.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-14 23:02:16.779173 papers_dl-0.0.1/tests/
--rw-r--r--   0 ben        (501) staff       (20)      806 2024-04-14 01:42:33.000000 papers_dl-0.0.1/tests/test.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-15 18:11:45.120850 papers_dl-0.0.2/
+-rw-r--r--   0 ben        (501) staff       (20)     1070 2024-03-23 22:45:07.000000 papers_dl-0.0.2/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)     1288 2024-04-15 18:11:45.120642 papers_dl-0.0.2/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      755 2024-04-14 23:03:56.000000 papers_dl-0.0.2/README.md
+-rw-r--r--   0 ben        (501) staff       (20)      603 2024-04-15 18:11:14.000000 papers_dl-0.0.2/pyproject.toml
+-rw-r--r--   0 ben        (501) staff       (20)       38 2024-04-15 18:11:45.120908 papers_dl-0.0.2/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-15 18:11:45.119305 papers_dl-0.0.2/src/
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-15 18:11:45.120421 papers_dl-0.0.2/src/papers_dl.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     1288 2024-04-15 18:11:45.000000 papers_dl-0.0.2/src/papers_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      221 2024-04-15 18:11:45.000000 papers_dl-0.0.2/src/papers_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2024-04-15 18:11:45.000000 papers_dl-0.0.2/src/papers_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       13 2024-04-15 18:11:45.000000 papers_dl-0.0.2/src/papers_dl.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)      353 2024-04-15 17:55:03.000000 papers_dl-0.0.2/src/parse.py
+-rw-r--r--   0 ben        (501) staff       (20)    10431 2024-04-14 01:36:31.000000 papers_dl-0.0.2/src/scihub.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-15 18:11:45.120081 papers_dl-0.0.2/tests/
+-rw-r--r--   0 ben        (501) staff       (20)     2130 2024-04-15 17:59:50.000000 papers_dl-0.0.2/tests/test.py
```

### Comparing `papers_dl-0.0.1/LICENSE` & `papers_dl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.1/PKG-INFO` & `papers_dl-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: papers-dl
-Version: 0.0.1
+Version: 0.0.2
 Summary: A command line application for downloading scientific papers
 Author-email: Ben Muthalaly <benmuthalaly@gmail.com>
 Project-URL: Homepage, https://github.com/benmuth/papers-dl
 Project-URL: Issues, https://github.com/benmuth/papers-dl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Overview
-`sci-dl` is a command line application for downloading scientific papers.
+`papers-dl` is a command line application for downloading scientific papers.
 
 ## Usage
 
-`python scihub-extractor.py -d <DOI|URL> -o <output directory>`
+`python papers-dl.py -d <DOI|URL> -o <output directory>`
 
 or
 
-`python scihub-extractor.py -f <text file with newline separated DOIs|URLs> -o <output directory>`
+`python papers-dl.py -f <text file with newline separated DOIs|URLs> -o <output directory>`
 
 It should either
 
 - download the paper directly identified by the DOI or URL you gave it
 - if you gave it a URL but it can't directly find a paper through it, then it will parse the page's HTML for DOIs and attempt to download all DOIs that are found.
 
 In the second case, we can probably be smarter about only downloading the DOIs intended (based on title or something?), but it's pretty dumb right now.
```

### Comparing `papers_dl-0.0.1/README.md` & `papers_dl-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Overview
-`sci-dl` is a command line application for downloading scientific papers.
+`papers-dl` is a command line application for downloading scientific papers.
 
 ## Usage
 
-`python scihub-extractor.py -d <DOI|URL> -o <output directory>`
+`python papers-dl.py -d <DOI|URL> -o <output directory>`
 
 or
 
-`python scihub-extractor.py -f <text file with newline separated DOIs|URLs> -o <output directory>`
+`python papers-dl.py -f <text file with newline separated DOIs|URLs> -o <output directory>`
 
 It should either
 
 - download the paper directly identified by the DOI or URL you gave it
 - if you gave it a URL but it can't directly find a paper through it, then it will parse the page's HTML for DOIs and attempt to download all DOIs that are found.
 
 In the second case, we can probably be smarter about only downloading the DOIs intended (based on title or something?), but it's pretty dumb right now.
```

### Comparing `papers_dl-0.0.1/pyproject.toml` & `papers_dl-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "papers-dl"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ben Muthalaly", email="benmuthalaly@gmail.com" },
 ]
 description = "A command line application for downloading scientific papers"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `papers_dl-0.0.1/src/papers_dl.egg-info/PKG-INFO` & `papers_dl-0.0.2/src/papers_dl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: papers-dl
-Version: 0.0.1
+Version: 0.0.2
 Summary: A command line application for downloading scientific papers
 Author-email: Ben Muthalaly <benmuthalaly@gmail.com>
 Project-URL: Homepage, https://github.com/benmuth/papers-dl
 Project-URL: Issues, https://github.com/benmuth/papers-dl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Overview
-`sci-dl` is a command line application for downloading scientific papers.
+`papers-dl` is a command line application for downloading scientific papers.
 
 ## Usage
 
-`python scihub-extractor.py -d <DOI|URL> -o <output directory>`
+`python papers-dl.py -d <DOI|URL> -o <output directory>`
 
 or
 
-`python scihub-extractor.py -f <text file with newline separated DOIs|URLs> -o <output directory>`
+`python papers-dl.py -f <text file with newline separated DOIs|URLs> -o <output directory>`
 
 It should either
 
 - download the paper directly identified by the DOI or URL you gave it
 - if you gave it a URL but it can't directly find a paper through it, then it will parse the page's HTML for DOIs and attempt to download all DOIs that are found.
 
 In the second case, we can probably be smarter about only downloading the DOIs intended (based on title or something?), but it's pretty dumb right now.
```

### Comparing `papers_dl-0.0.1/src/scihub.py` & `papers_dl-0.0.2/src/scihub.py`

 * *Files identical despite different names*

