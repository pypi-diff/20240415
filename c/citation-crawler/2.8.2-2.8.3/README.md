# Comparing `tmp/citation_crawler-2.8.2.tar.gz` & `tmp/citation_crawler-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_crawler-2.8.2.tar", last modified: Sat Mar 23 18:37:50 2024, max compression
+gzip compressed data, was "citation_crawler-2.8.3.tar", last modified: Mon Apr 15 01:11:18 2024, max compression
```

## Comparing `citation_crawler-2.8.2.tar` & `citation_crawler-2.8.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:37:50.093005 citation_crawler-2.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-03-23 18:37:50.093005 citation_crawler-2.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:37:50.089005 citation_crawler-2.8.2/citation_crawler/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/citation_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/citation_crawler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/citation_crawler/arg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:37:50.089005 citation_crawler-2.8.2/citation_crawler/crawlers/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/citation_crawler/crawlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/citation_crawler/crawlers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/citation_crawler/crawlers/ss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/citation_crawler/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:37:50.093005 citation_crawler-2.8.2/citation_crawler/init/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/citation_crawler/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/citation_crawler/init/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/citation_crawler/items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:37:50.093005 citation_crawler-2.8.2/citation_crawler/summarizers/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/citation_crawler/summarizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/citation_crawler/summarizers/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/citation_crawler/summarizers/nx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:37:50.089005 citation_crawler-2.8.2/citation_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-03-23 18:37:50.000000 citation_crawler-2.8.2/citation_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-23 18:37:50.000000 citation_crawler-2.8.2/citation_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 18:37:50.000000 citation_crawler-2.8.2/citation_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-23 18:37:50.000000 citation_crawler-2.8.2/citation_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-23 18:37:50.000000 citation_crawler-2.8.2/citation_crawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 18:37:50.093005 citation_crawler-2.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-23 18:37:43.000000 citation_crawler-2.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:18.207524 citation_crawler-2.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-15 01:11:18.207524 citation_crawler-2.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:18.203524 citation_crawler-2.8.3/citation_crawler/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/arg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:18.207524 citation_crawler-2.8.3/citation_crawler/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/crawlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/crawlers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/crawlers/ss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:18.207524 citation_crawler-2.8.3/citation_crawler/init/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/init/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:18.207524 citation_crawler-2.8.3/citation_crawler/summarizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/summarizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/summarizers/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/summarizers/nx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:18.203524 citation_crawler-2.8.3/citation_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-15 01:11:17.000000 citation_crawler-2.8.3/citation_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 01:11:18.000000 citation_crawler-2.8.3/citation_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 01:11:17.000000 citation_crawler-2.8.3/citation_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 01:11:17.000000 citation_crawler-2.8.3/citation_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 01:11:17.000000 citation_crawler-2.8.3/citation_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 01:11:18.207524 citation_crawler-2.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/setup.py
```

### Comparing `citation_crawler-2.8.2/LICENSE` & `citation_crawler-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.2/PKG-INFO` & `citation_crawler-2.8.3/citation_crawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: citation_crawler
-Version: 2.8.2
+Name: citation-crawler
+Version: 2.8.3
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citation_crawler-2.8.2/README.md` & `citation_crawler-2.8.3/README.md`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.2/citation_crawler/__main__.py` & `citation_crawler-2.8.3/citation_crawler/__main__.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.2/citation_crawler/arg.py` & `citation_crawler-2.8.3/citation_crawler/arg.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.2/citation_crawler/crawlers/common.py` & `citation_crawler-2.8.3/citation_crawler/crawlers/common.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.2/citation_crawler/crawlers/ss.py` & `citation_crawler-2.8.3/citation_crawler/crawlers/ss.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,14 +104,18 @@
     def doi(self) -> Optional[str]:
         if 'externalIds' in self.data and self.data['externalIds'] and 'DOI' in self.data['externalIds']:
             doi = self.data['externalIds']['DOI']
             u = urlparse(doi)
             doi = re.sub(r"^/+", "", u.path)
             return doi
 
+    def abstract(self) -> Optional[int]:
+        if 'abstract' in self.data:
+            return self.data['abstract']
+
     async def _get_authors_from_author_data(self) -> Iterable[Author]:
         if not self.author_data:
             authors = []
             async for author in get_authors(self.paperId()):
                 authors.append(author)
             self.author_data = authors
         for author in self.author_data:
@@ -142,15 +146,15 @@
             yield paper
 
     async def get_citations(self) -> Iterable[Paper]:
         async for paper in get_citations(self.paperId()):
             yield paper
 
 
-fields_references = f"title,year,authors,externalIds,publicationTypes,journal"
+fields_references = f"title,abstract,year,authors,externalIds,publicationTypes,journal"
 root_references = f"semanticscholar/references--{fields_references.replace(',', '-')}"
 root_citations = f"semanticscholar/citations--{fields_references.replace(',', '-')}"
 
 
 async def get_references(paperId: str) -> Iterable[SSPaper]:
     cache_days = getenv_int('CITATION_CRAWLER_MAX_CACHE_DAYS_REFERENCES')
     cache_days = cache_days if cache_days is not None else -1
@@ -188,15 +192,15 @@
     text = await download_item(url, path, cache_days, paper_is_valid)
     if not text:
         return
     return json.loads(text)
 
 
 fields_authors_sub = ','.join([("authors." + f) for f in fields_authors.split(',')])
-fields_paper = f"title,year,publicationDate,{fields_authors_sub},externalIds,publicationTypes,journal"
+fields_paper = f"title,abstract,year,publicationDate,{fields_authors_sub},externalIds,publicationTypes,journal"
 root_paper = f"semanticscholar/paper--{fields_paper.replace(',', '-')}"
 
 
 async def get_paper(paperId: str) -> Optional[SSPaper]:
     def paperId2path(paperId):
         return paperId.replace(":", "/")
     cache_days = getenv_int('CITATION_CRAWLER_MAX_CACHE_DAYS_PAPER')
```

### Comparing `citation_crawler-2.8.2/citation_crawler/graph.py` & `citation_crawler-2.8.3/citation_crawler/graph.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.2/citation_crawler/init/neo4j.py` & `citation_crawler-2.8.3/citation_crawler/init/neo4j.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.2/citation_crawler/items.py` & `citation_crawler-2.8.3/citation_crawler/items.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,18 @@
         return None
 
     @abc.abstractmethod
     def doi(self) -> Optional[str]:
         return None
 
     @abc.abstractmethod
+    def abstract(self) -> Optional[str]:
+        return None
+
+    @abc.abstractmethod
     async def authors(self) -> Iterable[Author]:
         return
 
     @abc.abstractmethod
     async def authors_kv(self) -> Iterable[Tuple[str, str]]:
         """key and correlated value to match authors"""
         return
@@ -87,11 +91,13 @@
             d['title_hash'] = self.title_hash()
         if self.year():
             d['year'] = self.year()
         if self.date():
             d['date'] = self.date()
         if self.doi():
             d['doi'] = self.doi()
+        if self.abstract():
+            d['abstract'] = self.abstract()
         d['authors'] = []
         async for author in self.authors():
             d['authors'].append(author.__dict__())
         return d
```

### Comparing `citation_crawler-2.8.2/citation_crawler/summarizers/neo4j.py` & `citation_crawler-2.8.3/citation_crawler/summarizers/neo4j.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 
 async def add_paper(tx, paper: Paper):
     n4jset = "MERGE (p:Publication {title_hash: $title_hash}) "\
         "SET p.title=$title, p.year=$year"
     if paper.doi():
         n4jset += ", p.doi=$doi"
+    if paper.abstract():
+        n4jset += ", p.abstract=$abstract"
     if paper.dblp_id():
         n4jset += ", p.dblp_key=$dblp_id"
     if paper.paperId():
         n4jset += ", p.paperId=$paperId"
     date = None
     if paper.date():
         try:
@@ -35,14 +37,15 @@
     await tx.run(n4jset,
                  title_hash=paper.title_hash(),
                  title=paper.title(),
                  year=paper.year(),
                  paperId=paper.paperId(),
                  dblp_id=paper.dblp_id(),
                  doi=paper.doi(),
+                 abstract=paper.abstract(),
                  date=date)
 
 
 async def add_reference(tx, a: Paper, b: Paper):
     await tx.run("MERGE (a:Publication {title_hash: $a}) "
                  "MERGE (b:Publication {title_hash: $b}) "
                  "MERGE (a)-[:CITE]->(b)",
```

### Comparing `citation_crawler-2.8.2/citation_crawler/summarizers/nx.py` & `citation_crawler-2.8.3/citation_crawler/summarizers/nx.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.2/citation_crawler.egg-info/PKG-INFO` & `citation_crawler-2.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: citation-crawler
-Version: 2.8.2
+Name: citation_crawler
+Version: 2.8.3
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citation_crawler-2.8.2/citation_crawler.egg-info/SOURCES.txt` & `citation_crawler-2.8.3/citation_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.2/setup.py` & `citation_crawler-2.8.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'citation_crawler.crawlers': 'citation_crawler/crawlers',
     'citation_crawler.summarizers': 'citation_crawler/summarizers',
     'citation_crawler.init': 'citation_crawler/init',
 }
 
 setup(
     name='citation_crawler',
-    version='2.8.2',
+    version='2.8.3',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/citation-crawler',
     description=u'Asynchronous high-concurrency citation crawler, use with caution!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

