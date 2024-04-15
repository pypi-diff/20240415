# Comparing `tmp/miuc-0.2.2.tar.gz` & `tmp/miuc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miuc-0.2.2.tar", max compression
+gzip compressed data, was "miuc-0.2.3.tar", max compression
```

## Comparing `miuc-0.2.2.tar` & `miuc-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 miuc-0.2.2/LICENSE
--rw-r--r--   0        0        0       33 2023-06-29 02:08:22.449672 miuc-0.2.2/miuc/__init__.py
--rw-r--r--   0        0        0      966 2024-02-24 08:17:15.166329 miuc-0.2.2/miuc/main.py
--rw-r--r--   0        0        0    35508 2024-02-28 10:22:03.999469 miuc-0.2.2/miuc/site_processor.py
--rw-r--r--   0        0        0     2412 2023-07-06 01:11:49.781049 miuc-0.2.2/miuc/utils.py
--rw-r--r--   0        0        0     2484 2024-02-26 13:53:21.032147 miuc-0.2.2/miuc/web_parser.py
--rw-r--r--   0        0        0      510 2024-02-28 10:22:08.047592 miuc-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1587 2023-07-06 02:06:31.528835 miuc-0.2.2/README.md
--rw-r--r--   0        0        0     2378 1970-01-01 00:00:00.000000 miuc-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 miuc-0.2.3/LICENSE
+-rw-r--r--   0        0        0       33 2023-06-29 02:08:22.449672 miuc-0.2.3/miuc/__init__.py
+-rw-r--r--   0        0        0      966 2024-02-24 08:17:15.166329 miuc-0.2.3/miuc/main.py
+-rw-r--r--   0        0        0    35503 2024-04-15 12:19:03.981850 miuc-0.2.3/miuc/site_processor.py
+-rw-r--r--   0        0        0     2412 2023-07-06 01:11:49.781049 miuc-0.2.3/miuc/utils.py
+-rw-r--r--   0        0        0     2734 2024-04-15 12:20:27.118118 miuc-0.2.3/miuc/web_parser.py
+-rw-r--r--   0        0        0      510 2024-04-15 12:21:10.807265 miuc-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1587 2023-07-06 02:06:31.528835 miuc-0.2.3/README.md
+-rw-r--r--   0        0        0     2378 1970-01-01 00:00:00.000000 miuc-0.2.3/PKG-INFO
```

### Comparing `miuc-0.2.2/LICENSE` & `miuc-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `miuc-0.2.2/miuc/main.py` & `miuc-0.2.3/miuc/main.py`

 * *Files identical despite different names*

### Comparing `miuc-0.2.2/miuc/site_processor.py` & `miuc-0.2.3/miuc/site_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -756,15 +756,15 @@
 
 
 class Weixin(Processor):
     def __init__(self, max_time_limit: int = 5) -> None:
         super().__init__(max_time_limit)
         self.site = "微信公众号"
         self.article_name = None
-        self.urls_re = [r"^https://mp\.weixin\.qq\.com/s/(?P<id>.*?)/?$"]
+        self.urls_re = [r"^https://mp\.weixin\.qq\.com/s/?(.*?)/?$"]
 
     def parse(self, res: Match) -> str:
         pattern = r'<h1 class="rich_media_title " id="activity-name">(.*?)</h1>'
         self.article_name = self.get_element_match(pattern, re.S).strip()
 
     def format(self):
         title = self.site
```

### Comparing `miuc-0.2.2/miuc/utils.py` & `miuc-0.2.3/miuc/utils.py`

 * *Files identical despite different names*

### Comparing `miuc-0.2.2/miuc/web_parser.py` & `miuc-0.2.3/miuc/web_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     r"^https://raw\.githubusercontent\.com.*": Githubusercontent,
     r"^https://www\.cnblogs\.com.*": CNblog,
     r"^https://www\.jianshu\.com.*": Jianshu,
     r"^https://cloud\.tencent\.com.*": TecentCloud,
     r"^https://book\.douban\.com.*": Douban,
     r"^https://juejin\.cn.*": Juejin,
     r"^https://en\.wikipedia\.org/wiki/.*": Wiki,
-    r"^https://mp.weixin\.qq\.com/s/.*": Weixin,
+    r"^https://mp.weixin\.qq\.com/s/?.*": Weixin,
     r"^https://www\.geeksforgeeks\.org/.*": Geeksforgeeks,
     r"^https://sourceforge\.net/projects/.*": SourceForge,
     r"^https://marketplace\.visualstudio\.com/items\?itemName=.*": VscodeExtension,
     r"^https://xie\.infoq\.cn/.*": InfoQ,
     r"^https://www\.51cto\.com/.*": CTO51,
     r"^https://www\.sohu\.com/.*": Souhu,
     r"^https://dl\.acm\.org/doi/.*": Acm,
@@ -48,14 +48,15 @@
 }
 
 
 def parse_url(url: str, max_time_limit: int = 5) -> str:
     """
     parse url and return the tite for the page
     """
+    url = "https://mp.weixin.qq.com/s?__biz=Mzg2OTc0ODAzMw==&mid=2247506713&idx=1&sn=38ca5f3af28d741b46e0197a5decd0a2&chksm=ce9ac737f9ed4e21f8a39efd85be7390863ab13faa9bafc1f031f1adef8b0c2b561f04302b20&scene=178&cur_album_id=2519398872503353344#rd"
     res = re.match(r"^https://link\.zhihu\.com/\?target=(?P<url>.*?)/?$", url)
     if res:
         return parse_url(unquote(res.group("url")), max_time_limit)
     # first check the url whether in specific sites
     try:
         for specific_page_url in SPECIFIC_SITES:
             if re.match(specific_page_url, url):
```

### Comparing `miuc-0.2.2/README.md` & `miuc-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `miuc-0.2.2/PKG-INFO` & `miuc-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miuc
-Version: 0.2.2
+Version: 0.2.3
 Summary: Markdown Intelligence Url Complete
 Home-page: https://github.com/luzhixing12345/miuc
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

