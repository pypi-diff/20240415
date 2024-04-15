# Comparing `tmp/hltv_async_api-0.4.5.tar.gz` & `tmp/hltv_async_api-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.4.5.tar", last modified: Tue Apr  9 13:52:25 2024, max compression
+gzip compressed data, was "hltv_async_api-0.4.6.tar", last modified: Mon Apr 15 17:11:15 2024, max compression
```

## Comparing `hltv_async_api-0.4.5.tar` & `hltv_async_api-0.4.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 13:52:25.781702 hltv_async_api-0.4.5/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.4.5/LICENSE
--rw-rw-rw-   0        0        0    11823 2024-04-09 13:52:25.779683 hltv_async_api-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0    11200 2024-04-09 13:03:53.000000 hltv_async_api-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 13:52:25.767687 hltv_async_api-0.4.5/hltv_async_api/
--rw-rw-rw-   0        0        0      124 2024-04-09 13:52:23.000000 hltv_async_api-0.4.5/hltv_async_api/__init__.py
--rw-rw-rw-   0        0        0    33567 2024-04-09 13:51:53.000000 hltv_async_api-0.4.5/hltv_async_api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:52:25.777685 hltv_async_api-0.4.5/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0    11823 2024-04-09 13:52:25.000000 hltv_async_api-0.4.5/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-09 13:52:25.000000 hltv_async_api-0.4.5/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 13:52:25.000000 hltv_async_api-0.4.5/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-09 13:52:25.000000 hltv_async_api-0.4.5/hltv_async_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      537 2024-04-09 13:52:23.000000 hltv_async_api-0.4.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 13:52:25.782685 hltv_async_api-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-04-09 13:52:23.000000 hltv_async_api-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:11:15.843173 hltv_async_api-0.4.6/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0    11823 2024-04-15 17:11:15.842171 hltv_async_api-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11200 2024-04-09 13:03:53.000000 hltv_async_api-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 17:11:15.831171 hltv_async_api-0.4.6/hltv_async_api/
+-rw-rw-rw-   0        0        0      124 2024-04-15 17:06:53.000000 hltv_async_api-0.4.6/hltv_async_api/__init__.py
+-rw-rw-rw-   0        0        0    33435 2024-04-15 09:56:27.000000 hltv_async_api-0.4.6/hltv_async_api/aiohltv.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:11:15.841173 hltv_async_api-0.4.6/hltv_async_api.egg-info/
+-rw-rw-rw-   0        0        0    11823 2024-04-15 17:11:15.000000 hltv_async_api-0.4.6/hltv_async_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-15 17:11:15.000000 hltv_async_api-0.4.6/hltv_async_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:11:15.000000 hltv_async_api-0.4.6/hltv_async_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 17:11:15.000000 hltv_async_api-0.4.6/hltv_async_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      537 2024-04-15 17:06:53.000000 hltv_async_api-0.4.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 17:11:15.843173 hltv_async_api-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      947 2024-04-15 17:06:53.000000 hltv_async_api-0.4.6/setup.py
```

### Comparing `hltv_async_api-0.4.5/LICENSE` & `hltv_async_api-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.4.5/PKG-INFO` & `hltv_async_api-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.4.5
+Version: 0.4.6
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv_async_api-0.4.5/README.md` & `hltv_async_api-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.4.5/hltv_async_api/aiohltv.py` & `hltv_async_api-0.4.6/hltv_async_api/aiohltv.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         self.logger.debug('Creating Session')
         self.session = ClientSession()
 
     async def close_session(self):
         if self.session:
             self.logger.debug('Closing Session')
             await self.session.close()
+            self.session = None
 
     def config(self, max_delay: int | None = None,
                timeout: int | None = None,
                use_proxy: bool | None = None,
                proxy_file_path: str | None = None,
                proxy_list: list | None = None,
                debug: bool | None = None,
@@ -111,15 +112,16 @@
             self.logger.debug(f'Removing proxy {self.PROXY_LIST[0]}')
             self.PROXY_LIST = self.PROXY_LIST[1:]
         else:
             self.logger.debug(f"Switching proxy {self.PROXY_LIST[0] if self.PROXY_LIST[0] else 'No Proxy'}")
             self.PROXY_LIST = self.PROXY_LIST[1:] + [(self.PROXY_LIST[0])]
             self.logger.info(f"New proxy: {self.PROXY_LIST[0] if self.PROXY_LIST[0] else 'No Proxy'}")
 
-    def _f(self, result):
+    @staticmethod
+    def _f(result):
         return BeautifulSoup(result, "lxml")
 
     async def _cloudflare_check(self, result) -> bool:
         page = self._f(result)
         challenge_page = page.find(id="challenge-error-title")
         if challenge_page is not None:
             if "Enable JavaScript and cookies to continue" in challenge_page.get_text():
@@ -169,43 +171,40 @@
     async def _fetch(self, url, delay: int = 0):
         if not self.session:
             await self._create_session()
 
         status = False
         try_ = 1
         result = None
+
+        # parse until success or not maxretries
         while (not status) and (try_ != self.max_retries):
             self.logger.debug(f'Trying connect to {url}, try {try_}/{self.max_retries}')
 
             # if status = True, result = page,
-            # if status = False result = delay (default=0)
+            # if status = False, result = delay (default=0)
             status, result = await self._parse(url, delay)
 
             if not status and result:
                 delay = result
             try_ += 1
 
         # After Parse
         if not self.TRUE_SESSION:
-            # Automaticaly close session after parse
+            # Automatically close session after parse
             await self.close_session()
-            self.session = None
 
         if status:
             loop = get_running_loop()
             parsed = await loop.run_in_executor(None, partial(self._f, result))
             return parsed
         else:
             self.logger.error('Connection failed')
             return None
 
-    def save_error(self, page):
-        with open("error.html", "w") as file:
-            file.write(page.prettify())
-
     @staticmethod
     def _normalize_date(parts) -> str:
         month_abbreviations = {
             'Jan': '1', 'Feb': '2', 'Mar': '3', 'Apr': '4',
             'May': '5', 'Jun': '6', 'Jul': '7', 'Aug': '8',
             'Sep': '9', 'Oct': '10', 'Nov': '11', 'Dec': '12'
         }
@@ -340,15 +339,15 @@
                     nickname = re.findall(r"'(.*?)'", player_name)[0]
 
                     kd = player.find('td', class_='kd').text.strip()
                     adr = player.find('td', class_='adr').text.strip()
                     rating = player.find('td', class_='rating').text.strip()
                     stats_.append({
                         'id': player_id,
-                        'name': nickname,
+                        'nickname': nickname,
                         'kd': kd,
                         'adr': adr,
                         'rating': rating
                     })
 
         if status == "LIVE":
             for map in maps:
@@ -400,36 +399,33 @@
         if not r:
             return
 
         match_results = []
 
         for result in r.find("div", {'class', 'results-holder'}).find_all("div", {'class', 'results-sublist'}):
             date = result.find("span", class_="standard-headline").text.strip()
-            match_date = []
             for match in result.find_all("a", class_="a-reset"):
                 id_ = match['href'].split('/')[2]
                 teams = match.find_all("div", class_="team")
                 team1 = teams[0].text.strip()
                 team2 = teams[1].text.strip()
 
                 scores = match.find("td", class_="result-score").text.strip().split('-')
                 score_t1 = scores[0].strip()
                 score_t2 = scores[1].strip()
 
-                match_date.append({
+                # add team ids?
+                match_results.append({
                     'id': id_,
+                    'date': date,
                     'team1': team1,
                     'team2': team2,
                     'score1': score_t1,
                     'score2': score_t2,
                 })
-            match_results.append({
-                'date': date,
-                'matches': match_date,
-            })
         return match_results
 
     async def get_event_matches(self, event_id: str | int, days: int = 1):
         r = await self._fetch("https://www.hltv.org/events/" + str(event_id) + "/matches")
         if not r:
             return
 
@@ -511,15 +507,15 @@
 
                 event_end_date = self._normalize_date(
                     event.find_all('span', {'data-time-format': 'MMM do'})[1].text.strip().split())
                 event_id = event['href'].split('/')[-2]
 
                 events.append({
                     'id': event_id,
-                    'name': event_name,
+                    'title': event_name,
                     'start_date': event_start_date,
                     'end_date': event_end_date,
                 })
         except AttributeError:
             pass
 
         return events
@@ -549,15 +545,15 @@
 
                 event_end_date = self._normalize_date(
                     event.find_all('span', {'data-time-format': 'MMM do'})[1].text.strip().split())
                 event_id = event['href'].split('/')[-2]
 
                 events.append({
                     'id': event_id,
-                    'name': event_name,
+                    'title': event_name,
                     'start_date': event_start_date,
                     'end_date': event_end_date,
                 })
 
         if future:
             for i, big_event_div in enumerate(r.find_all('div', {'class': 'big-events'}, start=1)):
                 for event in big_event_div.find_all('a', {'class': 'a-reset standard-box big-event'}):
```

### Comparing `hltv_async_api-0.4.5/hltv_async_api.egg-info/PKG-INFO` & `hltv_async_api-0.4.6/hltv_async_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.4.5
+Version: 0.4.6
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv_async_api-0.4.5/pyproject.toml` & `hltv_async_api-0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hltv_async_api"
-version = "0.4.5"
+version = "0.4.6"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hltv_async_api-0.4.5/setup.py` & `hltv_async_api-0.4.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hltv_async_api',
-    version='0.4.5',
+    version='0.4.6',
     author='akimerslys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
     packages=find_packages(),
@@ -18,14 +18,15 @@
         'beautifulsoup4==4.12.3',
         'frozenlist==1.4.1',
         'idna==3.6',
         'multidict==6.0.5',
         'lxml==5.2.0',
         'soupsieve==2.5',
         'yarl==1.9.4',
+        'pytz==2024.1',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

