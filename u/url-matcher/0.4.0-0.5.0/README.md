# Comparing `tmp/url-matcher-0.4.0.tar.gz` & `tmp/url_matcher-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "url-matcher-0.4.0.tar", last modified: Wed Apr  3 07:02:22 2024, max compression
+gzip compressed data, was "url_matcher-0.5.0.tar", last modified: Mon Apr 15 14:41:23 2024, max compression
```

## Comparing `url-matcher-0.4.0.tar` & `url_matcher-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:02:22.372842 url-matcher-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-03 07:02:14.000000 url-matcher-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-03 07:02:22.372842 url-matcher-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-03 07:02:14.000000 url-matcher-0.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 07:02:14.000000 url-matcher-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 07:02:22.372842 url-matcher-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-03 07:02:14.000000 url-matcher-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:02:22.368842 url-matcher-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-03 07:02:14.000000 url-matcher-0.4.0/tests/test_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-03 07:02:14.000000 url-matcher-0.4.0/tests/test_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:02:22.372842 url-matcher-0.4.0/url_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 07:02:14.000000 url-matcher-0.4.0/url_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 07:02:14.000000 url-matcher-0.4.0/url_matcher/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-03 07:02:14.000000 url-matcher-0.4.0/url_matcher/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-03 07:02:14.000000 url-matcher-0.4.0/url_matcher/matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-04-03 07:02:14.000000 url-matcher-0.4.0/url_matcher/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-03 07:02:14.000000 url-matcher-0.4.0/url_matcher/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:02:22.372842 url-matcher-0.4.0/url_matcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-03 07:02:22.000000 url-matcher-0.4.0/url_matcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-03 07:02:22.000000 url-matcher-0.4.0/url_matcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:02:22.000000 url-matcher-0.4.0/url_matcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 07:02:22.000000 url-matcher-0.4.0/url_matcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 07:02:22.000000 url-matcher-0.4.0/url_matcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:41:23.435384 url_matcher-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-15 14:41:09.000000 url_matcher-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-15 14:41:23.431384 url_matcher-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-15 14:41:09.000000 url_matcher-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 14:41:09.000000 url_matcher-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:41:23.435384 url_matcher-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-15 14:41:09.000000 url_matcher-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:41:23.431384 url_matcher-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-15 14:41:09.000000 url_matcher-0.5.0/tests/test_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-15 14:41:09.000000 url_matcher-0.5.0/tests/test_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:41:23.431384 url_matcher-0.5.0/url_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 14:41:09.000000 url_matcher-0.5.0/url_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 14:41:09.000000 url_matcher-0.5.0/url_matcher/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-15 14:41:09.000000 url_matcher-0.5.0/url_matcher/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-04-15 14:41:09.000000 url_matcher-0.5.0/url_matcher/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-04-15 14:41:09.000000 url_matcher-0.5.0/url_matcher/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-15 14:41:09.000000 url_matcher-0.5.0/url_matcher/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:41:23.431384 url_matcher-0.5.0/url_matcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-15 14:41:23.000000 url_matcher-0.5.0/url_matcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-15 14:41:23.000000 url_matcher-0.5.0/url_matcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:41:23.000000 url_matcher-0.5.0/url_matcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 14:41:23.000000 url_matcher-0.5.0/url_matcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 14:41:23.000000 url_matcher-0.5.0/url_matcher.egg-info/top_level.txt
```

### Comparing `url-matcher-0.4.0/LICENSE` & `url_matcher-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `url-matcher-0.4.0/PKG-INFO` & `url_matcher-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: url-matcher
-Version: 0.4.0
+Version: 0.5.0
 Summary: URL matching rules library to connect URLs with resources
 Home-page: https://github.com/zytedata/url-matcher
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `url-matcher-0.4.0/README.rst` & `url_matcher-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `url-matcher-0.4.0/setup.py` & `url_matcher-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `url-matcher-0.4.0/tests/test_matcher.py` & `url_matcher-0.5.0/tests/test_matcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
 def test_matcher_add_remove_get():
     matcher = URLMatcher()
     patterns = Patterns(["example.com"])
     matcher.add_or_update(1, patterns)
     assert matcher.match("http://example.com") == 1
     assert matcher.get(1) is patterns
+    assert list(matcher.match_universal()) == []
 
     patterns_3 = Patterns(["example.com/articles"])
     matcher.add_or_update(3, patterns_3)
     assert matcher.match("http://example.com/articles") == 3
     assert matcher.get(3) is patterns_3
 
     # Testing update
@@ -89,20 +90,22 @@
 
     # Testing universal patterns
     univ_patterns = Patterns([""])
     matcher.add_or_update(2, univ_patterns)
     assert matcher.match("http://example.com") == 2
     assert matcher.match("http://example.com/products") == 1
     assert matcher.get(2) is univ_patterns
+    assert list(matcher.match_universal()) == [2]
 
     # Removing a universal pattern
     matcher.remove(2)
     assert matcher.match("http://example.com") is None
     assert matcher.match("http://example.com/products") == 1
     assert matcher.get(2) is None
+    assert list(matcher.match_universal()) == []
 
     # Removing regular patterns
     matcher.remove(3)
     assert matcher.match("http://example.com/products") == 1
     assert matcher.match("http://example.com/articles") is None
     assert matcher.get(3) is None
 
@@ -157,7 +160,30 @@
 
     assert list(matcher.match_all("http://example.com")) == [1]
     assert list(matcher.match_all("http://foo.example.com")) == [2, 1]
     assert list(matcher.match_all("http://bar.example.com")) == [4, 1]
     assert list(matcher.match_all("http://example.com/products")) == [1]
     assert list(matcher.match_all("http://foo.example.com/products")) == [2, 1]
     assert list(matcher.match_all("http://bar.example.com/products")) == [3, 4, 1]
+
+
+def test_match_all_include_universal():
+    matcher = URLMatcher()
+    matcher.add_or_update(1, Patterns(include=["example.com"]))
+    matcher.add_or_update(2, Patterns(include=[]))
+    matcher.add_or_update(3, Patterns(include=["foo.example.com"]))
+    matcher.add_or_update(4, Patterns(include=[""]))
+    assert list(matcher.match_all("http://example.com")) == [1, 4, 2]
+    assert list(matcher.match_all("http://example.com", include_universal=False)) == [1]
+    assert list(matcher.match_all("http://foo.example.com")) == [3, 1, 4, 2]
+    assert list(matcher.match_all("http://foo.example.com", include_universal=False)) == [3, 1]
+    assert list(matcher.match_all("http://example.net")) == [4, 2]
+    assert list(matcher.match_all("http://example.net", include_universal=False)) == []
+
+
+def test_match_universal():
+    matcher = URLMatcher()
+    matcher.add_or_update(1, Patterns(include=["example.com"]))
+    matcher.add_or_update(2, Patterns(include=[]))
+    matcher.add_or_update(3, Patterns(include=["foo.example.com"]))
+    matcher.add_or_update(4, Patterns(include=[""]))
+    assert list(matcher.match_universal()) == [4, 2]
```

### Comparing `url-matcher-0.4.0/tests/test_patterns.py` & `url_matcher-0.5.0/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `url-matcher-0.4.0/url_matcher/example.py` & `url_matcher-0.5.0/url_matcher/example.py`

 * *Files identical despite different names*

### Comparing `url-matcher-0.4.0/url_matcher/matcher.py` & `url_matcher-0.5.0/url_matcher/matcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,14 +103,15 @@
             assert matcher.match("http://example.com/product/a_product.html") == 1
             assert matcher.match("http://other.com/a_different_page") == 2
 
         :param data: A map or a list of tuples with identifier, patterns pairs to
                      initialize the object from
         """
         self.matchers_by_domain: Dict[str, List[PatternsMatcher]] = {}
+        self.matchers_universal: List[PatternsMatcher] = []
         self.patterns: Dict[Any, Patterns] = {}
 
         if data:
             items = data.items() if isinstance(data, Mapping) else data
             for identifier, patterns in items:
                 self.add_or_update(identifier, patterns)
 
@@ -147,23 +148,29 @@
             self._del_matcher(domain, identifier)
         if patterns.is_universal_pattern():
             self._del_matcher("", identifier)
 
     def get(self, identifier: Any) -> Optional[Patterns]:
         return self.patterns.get(identifier)
 
-    def match(self, url: str) -> Optional[Any]:
-        return next(self.match_all(url), None)
+    def match(self, url: str, *, include_universal=True) -> Optional[Any]:
+        return next(self.match_all(url, include_universal=include_universal), None)
 
-    def match_all(self, url: str) -> Iterator[Any]:
+    def match_all(self, url: str, *, include_universal=True) -> Iterator[Any]:
         domain = get_domain(url)
-        for matcher in chain(self.matchers_by_domain.get(domain) or [], self.matchers_by_domain.get("") or []):
+        matchers: Iterable[PatternsMatcher] = self.matchers_by_domain.get(domain) or []
+        if include_universal:
+            matchers = chain(matchers, self.matchers_universal)
+        for matcher in matchers:
             if matcher.match(url):
                 yield matcher.identifier
 
+    def match_universal(self) -> Iterator[Any]:
+        return (m.identifier for m in self.matchers_universal)
+
     def _sort_domain(self, domain: str):
         """
         Sort all the rules within a domain so that the matching can be done in sequence:
         the first rule matching wins.
 
         A total ordering is defined. This is ensured by using including
         the identifier in the sorting criteria
@@ -175,23 +182,30 @@
         """
 
         def sort_key(matcher: PatternsMatcher) -> Tuple:
             sorted_includes = sorted(map(hierarchical_str, matcher.patterns.get_includes_for(domain)))
             return (matcher.patterns.priority, sorted_includes, matcher.identifier)
 
         self.matchers_by_domain[domain].sort(key=sort_key, reverse=True)
+        self.matchers_universal.sort(key=sort_key, reverse=True)
 
     def _del_matcher(self, domain: str, identifier: Any):
         matchers = self.matchers_by_domain[domain]
         for idx in range(len(matchers)):
             if matchers[idx].identifier == identifier:
                 del matchers[idx]
                 break
         if not matchers:
             del self.matchers_by_domain[domain]
+        for idx in range(len(self.matchers_universal)):
+            if self.matchers_universal[idx].identifier == identifier:
+                del self.matchers_universal[idx]
+                break
 
     def _add_matcher(self, domain: str, matcher: PatternsMatcher):
         # FIXME: This can be made much more efficient if we insert the data directly in order instead of resorting.
         # The bisect module could be used for this purpose.
         # I'm leaving it for the future as insertion time is not critical.
         self.matchers_by_domain.setdefault(domain, []).append(matcher)
+        if domain == "":
+            self.matchers_universal.append(matcher)
         self._sort_domain(domain)
```

### Comparing `url-matcher-0.4.0/url_matcher/patterns.py` & `url_matcher-0.5.0/url_matcher/patterns.py`

 * *Files identical despite different names*

### Comparing `url-matcher-0.4.0/url_matcher/util.py` & `url_matcher-0.5.0/url_matcher/util.py`

 * *Files identical despite different names*

### Comparing `url-matcher-0.4.0/url_matcher.egg-info/PKG-INFO` & `url_matcher-0.5.0/url_matcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: url-matcher
-Version: 0.4.0
+Version: 0.5.0
 Summary: URL matching rules library to connect URLs with resources
 Home-page: https://github.com/zytedata/url-matcher
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

