# Comparing `tmp/pub.tools-5.0.2.tar.gz` & `tmp/pub_tools-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pub.tools-5.0.2.tar", last modified: Wed Apr  3 17:10:34 2024, max compression
+gzip compressed data, was "pub_tools-5.0.3.tar", last modified: Mon Apr 15 17:24:07 2024, max compression
```

## Comparing `pub.tools-5.0.2.tar` & `pub_tools-5.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:34.686735 pub.tools-5.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 17:10:29.000000 pub.tools-5.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-03 17:10:34.686735 pub.tools-5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-03 17:10:29.000000 pub.tools-5.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:34.682736 pub.tools-5.0.2/pub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:34.686735 pub.tools-5.0.2/pub/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/citations.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/cooking.py
--rw-r--r--   0 runner    (1001) docker     (127)    22699 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/entrez.py
--rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/isbn.py
--rw-r--r--   0 runner    (1001) docker     (127)  1443107 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/journals.json
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/journals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:34.686735 pub.tools-5.0.2/pub/tools/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23689 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/tests/test_citations.py
--rw-r--r--   0 runner    (1001) docker     (127)    17851 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/tests/test_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    25755 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/tests/test_entrez.py
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/tests/test_journals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:34.686735 pub.tools-5.0.2/pub.tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-03 17:10:34.000000 pub.tools-5.0.2/pub.tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-03 17:10:34.000000 pub.tools-5.0.2/pub.tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:10:34.000000 pub.tools-5.0.2/pub.tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 17:10:34.000000 pub.tools-5.0.2/pub.tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 17:10:34.000000 pub.tools-5.0.2/pub.tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:10:34.686735 pub.tools-5.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:24:07.481336 pub_tools-5.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 17:24:03.000000 pub_tools-5.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-15 17:24:07.481336 pub_tools-5.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-15 17:24:03.000000 pub_tools-5.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:24:07.473336 pub_tools-5.0.3/pub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:24:07.477336 pub_tools-5.0.3/pub/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/citations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/cooking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/entrez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/isbn.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1443107 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/journals.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/journals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:24:07.481336 pub_tools-5.0.3/pub/tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24651 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/tests/test_citations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17851 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/tests/test_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25839 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/tests/test_entrez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pub/tools/tests/test_journals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:24:07.481336 pub_tools-5.0.3/pub.tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-15 17:24:07.000000 pub_tools-5.0.3/pub.tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-15 17:24:07.000000 pub_tools-5.0.3/pub.tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:24:07.000000 pub_tools-5.0.3/pub.tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 17:24:07.000000 pub_tools-5.0.3/pub.tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 17:24:07.000000 pub_tools-5.0.3/pub.tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-15 17:24:03.000000 pub_tools-5.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:24:07.481336 pub_tools-5.0.3/setup.cfg
```

### Comparing `pub.tools-5.0.2/PKG-INFO` & `pub_tools-5.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pub.tools
-Version: 5.0.2
+Version: 5.0.3
 Summary: Get publication metadata from NCBI's eUtils and generate citations.
 Author-email: Eric Wohnlich <wohnlice@imsweb.com>
 License: GPL
 Project-URL: homepage, https://github.com/imsweb/pub.tools
 Project-URL: documentation, https://imsweb.github.io/pub.tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `pub.tools-5.0.2/README.md` & `pub_tools-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.2/pub/tools/citations.py` & `pub_tools-5.0.3/pub/tools/citations.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.2/pub/tools/cooking.py` & `pub_tools-5.0.3/pub/tools/cooking.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.2/pub/tools/entrez.py` & `pub_tools-5.0.3/pub/tools/entrez.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             pubdate.get('Month', ''), pubdate.get('Day', '')) if i]))
 
     volume = book.get('Volume', '')
     volumetitle = book.get('VolumeTitle', '')
     edition = book.get('Edition', '')
     series = book.get('CollectionTitle', '')
     isbn = book.get('Isbn', '')
-    isbn = isbn[0] if isinstance(isbn, list) else isbn
+    isbn = isbn[0] if isbn and isinstance(isbn, list) else isbn
     elocation = book.get('ELocationID', '')
     medium = book.get('Medium', '')
     reportnum = book.get('ReportNumber', '')
 
     pmid = document['PMID']
 
     sections = []
@@ -378,27 +378,23 @@
     # Make sure pmids is a list, since that's what Entrez expects (and sets, for example, are not sliceable).
     total_time = time.time()
     if isinstance(pmids, set):
         pmids = list(pmids)
     start = 0
     while start < len(pmids):
         pmid_slice = pmids[start:start + config.MAX_PUBS]
-        try:
-            timer = time.time()
-            logger.info(
-                f'Fetching publications {start} through {min(len(pmids), start + config.MAX_PUBS)}...')
-            handle = Entrez.efetch(db="pubmed", id=pmid_slice, retmode="xml")
-            data = Entrez.read(handle, escape=escape)
-            logger.info(f'Fetched and read after {time.time() - timer:02}s')
-            for record in data['PubmedArticle'] + data['PubmedBookArticle']:
-                yield _parse_entrez_record(record, escape)
-            start += config.MAX_PUBS
-        except Exception as e:
-            logger.error(f'efetch failed: "{e}"')
-            raise PubToolsError(f"Something is wrong with Entrez or these PMIDs: {','.join(pmid_slice)}")
+        timer = time.time()
+        logger.info(
+            f'Fetching publications {start} through {min(len(pmids), start + config.MAX_PUBS)}...')
+        handle = Entrez.efetch(db="pubmed", id=pmid_slice, retmode="xml")
+        data = Entrez.read(handle, escape=escape)
+        logger.info(f'Fetched and read after {time.time() - timer:02}s')
+        for record in data['PubmedArticle'] + data['PubmedBookArticle']:
+            yield _parse_entrez_record(record, escape)
+        start += config.MAX_PUBS
     logger.info(f'Total publications retrieved in {time.time() - total_time:.02} seconds')
 
 
 def find_pmids(query):
     """
     Perform an ESearch and extract the pmids
```

### Comparing `pub.tools-5.0.2/pub/tools/formatting.py` & `pub_tools-5.0.3/pub/tools/formatting.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.2/pub/tools/isbn.py` & `pub_tools-5.0.3/pub/tools/isbn.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.2/pub/tools/journals.json` & `pub_tools-5.0.3/pub/tools/journals.json`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.2/pub/tools/journals.py` & `pub_tools-5.0.3/pub/tools/journals.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.2/pub/tools/schema.py` & `pub_tools-5.0.3/pub/tools/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,16 @@
     def process(self, escape=False):
         """
         This should be called after instantiation. This removes the Biopython StringElement class and
         escapes HTML where appropriate
         """
 
         def munge(val, escape=False):
+            if val is None:
+                return None
             if isinstance(val, list):
                 return [munge(v, escape) for v in val]
             elif isinstance(val, dict):
                 return {k: munge(v, escape) for k, v in val.items()}
             elif dataclasses.is_dataclass(val):
                 for f in dataclasses.fields(val):
                     setattr(val, f.name, munge(getattr(val, f.name), escape))
```

### Comparing `pub.tools-5.0.2/pub/tools/tests/test_citations.py` & `pub_tools-5.0.3/pub/tools/tests/test_citations.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,28 +54,32 @@
             pagination='345-7',
             pubmodel='Print',
             abstract=[],
             pubstatus='print',
             medium='',
             pmid=''
         )
-        citation = '<span class="citation">Wohnlich E, Carter G. My title. <i>Sample Journal</i> Jan 2007;4(5):345-7.</span>'
+        citation = '<span class="citation">Wohnlich E, Carter G. My title. <i>Sample Journal</i> ' \
+                   'Jan 2007;4(5):345-7.</span>'
         self.assertEqual(citation, journal_citation(html=True, publication=record))
 
         record.issue = ''
-        citation = '<span class="citation">Wohnlich E, Carter G. My title. <i>Sample Journal</i> Jan 2007;4:345-7.</span>'
+        citation = '<span class="citation">Wohnlich E, Carter G. My title. <i>Sample Journal</i> ' \
+                   'Jan 2007;4:345-7.</span>'
         self.assertEqual(citation, journal_citation(html=True, publication=record))
 
         record.issue = '5'
         record.volume = ''
-        citation = '<span class="citation">Wohnlich E, Carter G. My title. <i>Sample Journal</i> Jan 2007;(5):345-7.</span>'
+        citation = '<span class="citation">Wohnlich E, Carter G. My title. <i>Sample Journal</i> ' \
+                   'Jan 2007;(5):345-7.</span>'
         self.assertEqual(citation, journal_citation(html=True, publication=record))
 
         record.pagination = ''
-        citation = '<span class="citation">Wohnlich E, Carter G. My title. <i>Sample Journal</i> Jan 2007;(5).</span>'
+        citation = '<span class="citation">Wohnlich E, Carter G. My title. <i>Sample Journal</i> ' \
+                   'Jan 2007;(5).</span>'
         self.assertEqual(citation, journal_citation(html=True, publication=record))
 
         record.journal = ''
         citation = '<span class="citation">Wohnlich E, Carter G. My title. Jan 2007;(5).</span>'
         self.assertEqual(citation, journal_citation(html=True, publication=record))
 
     def test_journal_link_citation(self):
@@ -108,15 +112,16 @@
             pubdate='Jan 2007',
             volume='4',
             issue='5',
             pagination='345-7',
             pubmodel='Print',
             abstract=[Abstract(label='INTRO', text='my findings', nlmcategory='')],
         )
-        citation = '<span class="citation">Wohnlich E, Carter G. My title. <i>Sample Journal</i> Jan 2007;4(5):345-7. <br/>' \
+        citation = '<span class="citation">Wohnlich E, Carter G. My title. <i>Sample ' \
+                   'Journal</i> Jan 2007;4(5):345-7. <br/>' \
                    '<div class="citationAbstract"><p class="abstractHeader"><strong>Abstract</strong></p>' \
                    '<p>INTRO: my findings</p></div></span>'
         self.assertEqual(citation, journal_citation(html=True, use_abstract=True, publication=record))
 
     def test_book_citation(self):
         record = BookRecord(
             title='My title',
@@ -130,30 +135,34 @@
             edition='First Edition',
             pubdate='2007 Dec',
             publisher='Doubleday',
             pubplace='New York',
             pagination='243',
             series='My series',
         )
-        citation = '<span class="citation">Wohnlich E, Carter G. My title. First Edition. Van Halen E, editor. New York: ' \
+        citation = '<span class="citation">Wohnlich E, Carter G. My title. First Edition. ' \
+                   'Van Halen E, editor. New York: ' \
                    'Doubleday; 2007 Dec. p. 243. (My series)</span>'
         self.assertEqual(citation, book_citation(html=True, publication=record))
 
         record.pubdate = ''
-        citation = '<span class="citation">Wohnlich E, Carter G. My title. First Edition. Van Halen E, editor. New York: ' \
+        citation = '<span class="citation">Wohnlich E, Carter G. My title. First Edition. Van Halen E, ' \
+                   'editor. New York: ' \
                    'Doubleday. p. 243. (My series)</span>'
         self.assertEqual(citation, book_citation(html=True, publication=record))
 
         record.publisher = ''
-        citation = '<span class="citation">Wohnlich E, Carter G. My title. First Edition. Van Halen E, editor. New York. ' \
+        citation = '<span class="citation">Wohnlich E, Carter G. My title. First Edition. Van Halen E, ' \
+                   'editor. New York. ' \
                    'p. 243. (My series)</span>'
         self.assertEqual(citation, book_citation(html=True, publication=record))
 
         record.authors = []
-        citation = '<span class="citation">Van Halen E, editor. My title. First Edition. New York. p. 243. (My series)</span>'
+        citation = '<span class="citation">Van Halen E, editor. My title. First Edition. New York. p. 243. ' \
+                   '(My series)</span>'
         self.assertEqual(citation, book_citation(html=True, publication=record))
 
     def test_chapter_citation(self):
         record = ChapterRecord(
             title='My title',
             booktitle='My Book',
             authors=[
@@ -166,30 +175,34 @@
             edition='First Edition',
             pubdate='2007 Dec',
             publisher='Doubleday',
             pubplace='New York',
             pagination='243',
             series='My series',
         )
-        citation = '<span class="citation">Wohnlich E, Carter G. My title. In: Van Halen E, editor. My Book. First Edition. ' \
+        citation = '<span class="citation">Wohnlich E, Carter G. My title. In: Van Halen E, editor. ' \
+                   'My Book. First Edition. ' \
                    'New York: Doubleday; 2007 Dec. p. 243. (My series)</span>'
         self.assertEqual(citation, chapter_citation(html=True, publication=record))
 
         record.pubdate = ''
-        citation = '<span class="citation">Wohnlich E, Carter G. My title. In: Van Halen E, editor. My Book. First Edition. ' \
+        citation = '<span class="citation">Wohnlich E, Carter G. My title. In: Van Halen E, editor. ' \
+                   'My Book. First Edition. ' \
                    'New York: Doubleday. p. 243. (My series)</span>'
         self.assertEqual(citation, chapter_citation(html=True, publication=record))
 
         record.publisher = ''
-        citation = '<span class="citation">Wohnlich E, Carter G. My title. In: Van Halen E, editor. My Book. First Edition. ' \
+        citation = '<span class="citation">Wohnlich E, Carter G. My title. In: Van Halen E, editor. ' \
+                   'My Book. First Edition. ' \
                    'New York. p. 243. (My series)</span>'
         self.assertEqual(citation, chapter_citation(html=True, publication=record))
 
         record.authors = []
-        citation = '<span class="citation">Van Halen E, editor. My title. In: My Book. First Edition. New York. p. 243. ' \
+        citation = '<span class="citation">Van Halen E, editor. My title. In: My Book. First Edition. ' \
+                   'New York. p. 243. ' \
                    '(My series)</span>'
         self.assertEqual(citation, chapter_citation(html=True, publication=record))
 
     def test_conference_citation(self):
         record = ConferenceRecord(
             title='My title',
             authors=[
@@ -204,20 +217,22 @@
             conferencedate='2007 Dec',
             place='New York',
             pubdate='2008 Jan',
             publisher='Doubleday',
             pubplace='Boston',
             pagination='345',
         )
-        citation = '<span class="citation">Wohnlich E, Battle J. My title. Sagan C, Thorne K, editors. <i>Proceedings of Conference ' \
+        citation = '<span class="citation">Wohnlich E, Battle J. My title. Sagan C, Thorne K, editors. ' \
+                   '<i>Proceedings of Conference ' \
                    'name</i>; 2007 Dec; New York. Boston: Doubleday; 2008 Jan. p. 345.</span>'
         self.assertEqual(citation, conference_citation(html=True, publication=record))
 
         record.authors = []
-        citation = '<span class="citation">Sagan C, Thorne K, editors. My title. <i>Proceedings of Conference name</i>; 2007 Dec; New ' \
+        citation = '<span class="citation">Sagan C, Thorne K, editors. My title. <i>Proceedings of ' \
+                   'Conference name</i>; 2007 Dec; New ' \
                    'York. Boston: Doubleday; 2008 Jan. p. 345.</span>'
         self.assertEqual(citation, conference_citation(html=True, publication=record))
 
         record.authors = [
             Person(
                 last_name='Wohnlich',
                 first_name='',
@@ -226,25 +241,28 @@
             Person(
                 last_name='Battle',
                 first_name='',
                 initial='J'
             )
         ]
         record.pagination = ''
-        citation = '<span class="citation">Wohnlich E, Battle J. My title. Sagan C, Thorne K, editors. <i>Proceedings of Conference ' \
+        citation = '<span class="citation">Wohnlich E, Battle J. My title. Sagan C, Thorne K, editors. ' \
+                   '<i>Proceedings of Conference ' \
                    'name</i>; 2007 Dec; New York. Boston: Doubleday; 2008 Jan.</span>'
         self.assertEqual(citation, conference_citation(html=True, publication=record))
 
         record.publisher = ''
-        citation = '<span class="citation">Wohnlich E, Battle J. My title. Sagan C, Thorne K, editors. <i>Proceedings of Conference ' \
+        citation = '<span class="citation">Wohnlich E, Battle J. My title. Sagan C, Thorne K, editors. ' \
+                   '<i>Proceedings of Conference ' \
                    'name</i>; 2007 Dec; New York. Boston: 2008 Jan.</span>'
         self.assertEqual(citation, conference_citation(html=True, publication=record))
 
         record.pubplace = ''
-        citation = '<span class="citation">Wohnlich E, Battle J. My title. Sagan C, Thorne K, editors. <i>Proceedings of Conference ' \
+        citation = '<span class="citation">Wohnlich E, Battle J. My title. Sagan C, Thorne K, editors. ' \
+                   '<i>Proceedings of Conference ' \
                    'name</i>; 2007 Dec; New York. 2008 Jan.</span>'
         self.assertEqual(citation, conference_citation(html=True, publication=record))
 
     def test_monograph_citation(self):
         record = MonographRecord(
             title='My title',
             authors=[
@@ -255,44 +273,50 @@
             series='Series name',
             reportnum='5',
             weburl='http://plone.org',
             pubdate='2010 Feb',
             publisher='Doubleday',
             pubplace='Baltimore'
         )
-        citation = '<span class="citation">Wohnlich E, Battle J; My title. Series name. Hawking S, Wheeler J, editors. Baltimore: ' \
+        citation = '<span class="citation">Wohnlich E, Battle J; My title. Series name. Hawking S, ' \
+                   'Wheeler J, editors. Baltimore: ' \
                    'Doubleday; 2010 Feb. 5. Available at http://plone.org.</span>'
         self.assertEqual(citation, monograph_citation(html=True, publication=record))
 
         record.weburl = ''
-        citation = '<span class="citation">Wohnlich E, Battle J; My title. Series name. Hawking S, Wheeler J, editors. Baltimore: ' \
+        citation = '<span class="citation">Wohnlich E, Battle J; My title. Series name. Hawking S, ' \
+                   'Wheeler J, editors. Baltimore: ' \
                    'Doubleday; 2010 Feb. 5.</span>'
         self.assertEqual(citation, monograph_citation(html=True, publication=record))
 
         record.authors = []
-        citation = '<span class="citation">Hawking S, Wheeler J, editors. My title. Series name. Baltimore: Doubleday; 2010 Feb. ' \
+        citation = '<span class="citation">Hawking S, Wheeler J, editors. My title. Series name. ' \
+                   'Baltimore: Doubleday; 2010 Feb. ' \
                    '5.</span>'
         self.assertEqual(citation, monograph_citation(html=True, publication=record))
 
         record.authors = [
             Person(last_name='Wohnlich', first_name='', initial='E'),
             Person(last_name='Battle', first_name='', initial='J')
         ]
         record.title = ''
-        citation = '<span class="citation">Wohnlich E, Battle J; Series name. Hawking S, Wheeler J, editors. Baltimore: Doubleday; ' \
+        citation = '<span class="citation">Wohnlich E, Battle J; Series name. Hawking S, Wheeler J, ' \
+                   'editors. Baltimore: Doubleday; ' \
                    '2010 Feb. 5.</span>'
         self.assertEqual(citation, monograph_citation(html=True, publication=record))
 
         record.pubplace = ''
-        citation = '<span class="citation">Wohnlich E, Battle J; Series name. Hawking S, Wheeler J, editors. Doubleday; ' \
+        citation = '<span class="citation">Wohnlich E, Battle J; Series name. Hawking S, Wheeler J, ' \
+                   'editors. Doubleday; ' \
                    '2010 Feb. 5.</span>'
         self.assertEqual(citation, monograph_citation(html=True, publication=record))
 
         record.publisher = ''
-        citation = '<span class="citation">Wohnlich E, Battle J; Series name. Hawking S, Wheeler J, editors. 2010 Feb. 5.</span>'
+        citation = '<span class="citation">Wohnlich E, Battle J; Series name. Hawking S, Wheeler J, ' \
+                   'editors. 2010 Feb. 5.</span>'
         self.assertEqual(citation, monograph_citation(html=True, publication=record))
 
     def test_report_citation(self):
         record = ReportRecord(
             title='My title',
             authors=[
                 Person(last_name='Wohnlich', first_name='', initial='E'),
@@ -305,44 +329,50 @@
             series='Series name',
             reportnum='5',
             weburl='http://plone.org',
             pubdate='2010 Feb',
             publisher='Doubleday',
             pubplace='Baltimore'
         )
-        citation = '<span class="citation">Wohnlich E, Battle J. My title. Series name. Hawking S, Wheeler J, editors. Baltimore: ' \
+        citation = '<span class="citation">Wohnlich E, Battle J. My title. Series name. Hawking S, ' \
+                   'Wheeler J, editors. Baltimore: ' \
                    'Doubleday; 2010 Feb. 5. Available at http://plone.org.</span>'
         self.assertEqual(citation, report_citation(html=True, publication=record))
 
         record.weburl = ''
-        citation = '<span class="citation">Wohnlich E, Battle J. My title. Series name. Hawking S, Wheeler J, editors. Baltimore: ' \
+        citation = '<span class="citation">Wohnlich E, Battle J. My title. Series name. Hawking S, ' \
+                   'Wheeler J, editors. Baltimore: ' \
                    'Doubleday; 2010 Feb. 5.</span>'
         self.assertEqual(citation, report_citation(html=True, publication=record))
 
         record.authors = []
-        citation = '<span class="citation">Hawking S, Wheeler J, editors. My title. Series name. Baltimore: Doubleday; 2010 Feb. ' \
+        citation = '<span class="citation">Hawking S, Wheeler J, editors. My title. Series name. ' \
+                   'Baltimore: Doubleday; 2010 Feb. ' \
                    '5.</span>'
         self.assertEqual(citation, report_citation(html=True, publication=record))
 
         record.authors = [
             Person(last_name='Wohnlich', first_name='', initial='E'),
             Person(last_name='Battle', first_name='', initial='J')
         ]
         record.title = ''
-        citation = '<span class="citation">Wohnlich E, Battle J. Series name. Hawking S, Wheeler J, editors. Baltimore: Doubleday; ' \
+        citation = '<span class="citation">Wohnlich E, Battle J. Series name. Hawking S, Wheeler J, ' \
+                   'editors. Baltimore: Doubleday; ' \
                    '2010 Feb. 5.</span>'
         self.assertEqual(citation, report_citation(html=True, publication=record))
 
         record.pubplace = ''
-        citation = '<span class="citation">Wohnlich E, Battle J. Series name. Hawking S, Wheeler J, editors. Doubleday; 2010 ' \
+        citation = '<span class="citation">Wohnlich E, Battle J. Series name. Hawking S, Wheeler J, ' \
+                   'editors. Doubleday; 2010 ' \
                    'Feb. 5.</span>'
         self.assertEqual(citation, report_citation(html=True, publication=record))
 
         record.publisher = ''
-        citation = '<span class="citation">Wohnlich E, Battle J. Series name. Hawking S, Wheeler J, editors. 2010 Feb. 5.</span>'
+        citation = '<span class="citation">Wohnlich E, Battle J. Series name. Hawking S, Wheeler J, ' \
+                   'editors. 2010 Feb. 5.</span>'
         self.assertEqual(citation, report_citation(html=True, publication=record))
 
     def test_non_latin1(self):
         record = JournalRecord(
             title='My title',
             authors=[
                 Person(
@@ -358,15 +388,16 @@
             journal='Sample Journal',
             pubdate='Jan 2007',
             volume='4',
             issue='5',
             pagination='345-7',
             pubmodel='Print',
         )
-        citation = '<span class="citation">Wohnliché E, Carter G. My title. <i>Sample Journal</i> Jan 2007;4(5):345-7.</span>'
+        citation = '<span class="citation">Wohnliché E, Carter G. My title. <i>Sample Journal</i> ' \
+                   'Jan 2007;4(5):345-7.</span>'
         self.assertEqual(citation, journal_citation(html=True, publication=record))
 
     def test_html_chapter(self):
         record = ChapterRecord(
             title='Chapter 19. Estimating the Natural History of Breast Cancer from Bivariate Data on Age and '
                   'Tumor Size at Diagnosis',
             authors=[
@@ -391,15 +422,16 @@
             pagination='317-27',
             edition='',
             series='Wiley Series in Probability and Statistics',
             pubplace='New York',
             booktitle='Recent Advances in Quantitative Methods for Cancer and Human Health Risk Assessment',
             publisher='John Wiley & Sons, Ltd'
         )
-        citation = '<span class="citation">Zorin AV, Edler L, Hanin LG, Yakovlev AY. Chapter 19. Estimating the Natural History ' \
+        citation = '<span class="citation">Zorin AV, Edler L, Hanin LG, Yakovlev AY. Chapter 19. ' \
+                   'Estimating the Natural History ' \
                    'of Breast Cancer from Bivariate Data on Age and Tumor Size at Diagnosis. In: Edler L, ' \
                    'Kitsos CP, editors. Recent Advances in Quantitative Methods for Cancer and Human Health Risk ' \
                    'Assessment. New York: John Wiley &amp; Sons, Ltd; 2006 Mar 17. p. 317-27. (Wiley Series in ' \
                    'Probability and Statistics)</span>'
         self.assertEqual(citation, chapter_citation(html=True, publication=record))
 
     def test_linked_journal_citation(self):
@@ -422,35 +454,39 @@
             volume='4',
             issue='5',
             pagination='345-7',
             pubmodel='Print',
             abstract=[Abstract(label='INTRO', text='my findings', nlmcategory='')],
             pmid='12345678',
         )
-        citation = '<span class="citation">Wohnlich E, Carter G. <a class="citation-pubmed-link" href="https://pubmed.ncbi.nlm.nih.gov' \
+        citation = '<span class="citation">Wohnlich E, Carter G. <a class="citation-pubmed-link" ' \
+                   'href="https://pubmed.ncbi.nlm.nih.gov' \
                    '/12345678/">My title.</a> <i>Sample Journal</i> Jan 2007;4(5):345-7. <br/>' \
                    '<div class="citationAbstract"><p class="abstractHeader"><strong>Abstract</strong></p><p>INTRO: ' \
                    'my findings</p></div></span>'
         self.assertEqual(citation, journal_citation(html=True, link=True, use_abstract=True, publication=record))
 
     def test_citation_from_journal_dataclass(self):
         cit = publication_citation(publication=entrez.get_publication(pmid=12345678), html=True)
-        self.assertEqual(cit, '<span class="citation">Ministerial Meeting on Population of the Non-Aligned Movement (1993: '
+        self.assertEqual(cit, '<span class="citation">Ministerial Meeting on Population of '
+                              'the Non-Aligned Movement (1993: '
                               'Bali). Denpasar Declaration on Population and Development. <i>Integration</i> 1994 '
                               'Jun;(40):27-9.</span>')
 
     def test_citation_from_chapter_dataclass(self):
         cit = publication_citation(publication=entrez.get_publication(pmid=22593940), html=True)
-        self.assertEqual(cit, '<span class="citation">Kaefer CM, Milner JA, Benzie IFF, Wachtel-Galor S. Herbs and Spices in '
+        self.assertEqual(cit, '<span class="citation">Kaefer CM, Milner JA, Benzie IFF, '
+                              'Wachtel-Galor S. Herbs and Spices in '
                               'Cancer Prevention and Treatment. In: Herbal Medicine: Biomolecular and Clinical '
                               'Aspects. 2nd. Boca Raton (FL): CRC Press/Taylor &amp; Francis; 2011.</span>')
 
     def test_citation_from_book_dataclass(self):
         cit = publication_citation(publication=entrez.get_publication(pmid=12345678), html=True)
-        self.assertEqual(cit, '<span class="citation">Ministerial Meeting on Population of the Non-Aligned Movement (1993: '
+        self.assertEqual(cit, '<span class="citation">Ministerial Meeting on Population of the Non-Aligned '
+                              'Movement (1993: '
                               'Bali). Denpasar Declaration on Population and Development. <i>Integration</i> 1994 '
                               'Jun;(40):27-9.</span>')
 
     def test_citation_html_title(self):
         record = JournalRecord(
             title='My &lt;title&gt;',
             authors=[
@@ -464,15 +500,16 @@
             pagination='345-7',
             pubmodel='Print',
             abstract=[],
             pubstatus='print',
             medium='',
             pmid=''
         )
-        citation = '<span class="citation">Wohnlich E, Carter G. My &lt;title&gt;. <i>Sample Journal</i> Jan 2007;4(5):345-7.</span>'
+        citation = '<span class="citation">Wohnlich E, Carter G. My &lt;title&gt;. <i>Sample Journal</i> ' \
+                   'Jan 2007;4(5):345-7.</span>'
         self.assertEqual(citation, journal_citation(html=True, publication=record))
 
     def test_unescapted_journal_title(self):
         record = JournalRecord(
             title='My & title',
             authors=[
                 Person(last_name='Wohnlich', first_name='', initial='E'),
@@ -485,15 +522,16 @@
             pagination='345-7',
             pubmodel='Print',
             abstract=[],
             pubstatus='print',
             medium='',
             pmid=''
         )
-        citation = '<span class="citation">Wohnlich E, Carter G. My &amp; title. <i>Sample Journal</i> Jan 2007;4(5):345-7.</span>'
+        citation = '<span class="citation">Wohnlich E, Carter G. My &amp; title. <i>Sample Journal</i> ' \
+                   'Jan 2007;4(5):345-7.</span>'
         self.assertEqual(citation, journal_citation(html=True, publication=record))
 
     def test_bad_format_title(self):
         record = JournalRecord(
             title='My & &lt;title&gt;',
             authors=[
                 Person(last_name='Wohnlich', first_name='', initial='E'),
@@ -506,10 +544,11 @@
             pagination='345-7',
             pubmodel='Print',
             abstract=[],
             pubstatus='print',
             medium='',
             pmid=''
         )
-        citation = ('<span class="citation">Wohnlich E, Carter G. My &amp; &lt;title&gt;. <i>Sample Journal</i> Jan 2007;4(5):345-7.'
+        citation = ('<span class="citation">Wohnlich E, Carter G. My &amp; &lt;title&gt;. <i>Sample '
+                    'Journal</i> Jan 2007;4(5):345-7.'
                     '</span>')
         self.assertEqual(citation, journal_citation(html=True, publication=record))
```

### Comparing `pub.tools-5.0.2/pub/tools/tests/test_compatibility.py` & `pub_tools-5.0.3/pub/tools/tests/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.2/pub/tools/tests/test_entrez.py` & `pub_tools-5.0.3/pub/tools/tests/test_entrez.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,30 +353,33 @@
             # we didn't enter affiliations, it won't match
             self.compare_author(r, e)
 
     def test_print_electronic_pubmodel(self):
         """ Both dates should be stored and the citation reflect it """
         record = entrez.get_publication(pmid='10854512')
         self.assertEqual(citations.journal_citation(html=True, publication=record),
-                         '<span class="citation">Soon MS, Lin OS. Inflammatory fibroid polyp of the duodenum. <i>Surg Endosc</i> 2000 '
+                         '<span class="citation">Soon MS, Lin OS. Inflammatory fibroid polyp of the duodenum. '
+                         '<i>Surg Endosc</i> 2000 '
                          'Jan;14(1):86. Epub 1999 Nov 25.</span>')
 
     def test_electronic_print_pubmodel(self):
         """ Both dates should be stored but use electronic date for citation """
         record = entrez.get_publication(pmid='14729922')
         self.assertEqual(citations.journal_citation(html=True, publication=record),
-                         '<span class="citation">Edgar RC. Local homology recognition and distance measures in linear time using '
+                         '<span class="citation">Edgar RC. Local homology recognition and distance measures in '
+                         'linear time using '
                          'compressed '
                          'amino acid alphabets. <i>Nucleic Acids Res</i> 2004 Jan 16;32(1):380-5. Print 2004.</span>')
 
     def test_electronic_ecollection_pubmodel(self):
         """ Both dates should be stored but use electronic date for citation """
         record = entrez.get_publication(pmid='23372575')
         self.assertEqual(citations.journal_citation(html=True, publication=record),
-                         '<span class="citation">Wangari-Talbot J, Chen S. Genetics of melanoma. <i>Front Genet</i> 2013 '
+                         '<span class="citation">Wangari-Talbot J, Chen S. Genetics of melanoma. <i>Front '
+                         'Genet</i> 2013 '
                          'Jan 25;3:330. doi: '
                          '10.3389/fgene.2012.00330. eCollection 2012.</span>')
 
     def test_book_parse(self):
         """ Be able to parse a book """
         result = entrez.get_publication(pmid='22593940')
```

### Comparing `pub.tools-5.0.2/pub/tools/tests/test_formatting.py` & `pub_tools-5.0.3/pub/tools/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.2/pub/tools/tests/test_journals.py` & `pub_tools-5.0.3/pub/tools/tests/test_journals.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.2/pub.tools.egg-info/PKG-INFO` & `pub_tools-5.0.3/pub.tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pub.tools
-Version: 5.0.2
+Version: 5.0.3
 Summary: Get publication metadata from NCBI's eUtils and generate citations.
 Author-email: Eric Wohnlich <wohnlice@imsweb.com>
 License: GPL
 Project-URL: homepage, https://github.com/imsweb/pub.tools
 Project-URL: documentation, https://imsweb.github.io/pub.tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `pub.tools-5.0.2/pub.tools.egg-info/SOURCES.txt` & `pub_tools-5.0.3/pub.tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.2/pyproject.toml` & `pub_tools-5.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pub.tools"
-version = "5.0.2"
+version = "5.0.3"
 readme = "README.md"
 requires-python = ">=3.11"
 description = "Get publication metadata from NCBI's eUtils and generate citations."
 classifiers = [
           "Programming Language :: Python :: 3",
           "Topic :: Scientific/Engineering",
           "Topic :: Scientific/Engineering :: Bio-Informatics",
```

