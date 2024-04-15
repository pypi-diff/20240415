# Comparing `tmp/tweet-capture-0.2.4.tar.gz` & `tmp/tweet-capture-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweet-capture-0.2.4.tar", last modified: Sat Jan 27 15:07:14 2024, max compression
+gzip compressed data, was "tweet-capture-0.2.5.tar", last modified: Mon Apr 15 01:07:14 2024, max compression
```

## Comparing `tweet-capture-0.2.4.tar` & `tweet-capture-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-01-27 15:07:14.586148 tweet-capture-0.2.4/
--rw-rw-rw-   0        0        0     1085 2021-05-31 19:56:28.000000 tweet-capture-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     3238 2024-01-27 15:07:14.587155 tweet-capture-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2656 2023-04-06 14:53:44.000000 tweet-capture-0.2.4/README.md
--rw-rw-rw-   0        0        0       67 2023-04-06 14:53:44.000000 tweet-capture-0.2.4/requirements.txt
--rw-rw-rw-   0        0        0       86 2024-01-27 15:07:14.588147 tweet-capture-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1180 2024-01-27 15:06:40.000000 tweet-capture-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-27 15:07:14.569120 tweet-capture-0.2.4/tweet_capture.egg-info/
--rw-rw-rw-   0        0        0     3238 2024-01-27 15:07:14.000000 tweet-capture-0.2.4/tweet_capture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2024-01-27 15:07:14.000000 tweet-capture-0.2.4/tweet_capture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-27 15:07:14.000000 tweet-capture-0.2.4/tweet_capture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-01-27 15:07:14.000000 tweet-capture-0.2.4/tweet_capture.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2024-01-27 15:07:14.000000 tweet-capture-0.2.4/tweet_capture.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-01-27 15:07:14.000000 tweet-capture-0.2.4/tweet_capture.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-27 15:07:14.577635 tweet-capture-0.2.4/tweetcapture/
--rw-rw-rw-   0        0        0       60 2021-05-31 18:34:46.000000 tweet-capture-0.2.4/tweetcapture/__init__.py
--rw-rw-rw-   0        0        0     4199 2023-10-02 17:21:07.000000 tweet-capture-0.2.4/tweetcapture/cli.py
--rw-rw-rw-   0        0        0    18426 2024-01-27 15:06:40.000000 tweet-capture-0.2.4/tweetcapture/screenshot.py
-drwxrwxrwx   0        0        0        0 2024-01-27 15:07:14.584150 tweet-capture-0.2.4/tweetcapture/utils/
--rw-rw-rw-   0        0        0        0 2021-05-31 19:53:06.000000 tweet-capture-0.2.4/tweetcapture/utils/__init__.py
--rw-rw-rw-   0        0        0     1860 2023-09-22 19:05:50.000000 tweet-capture-0.2.4/tweetcapture/utils/utils.py
--rw-rw-rw-   0        0        0     2474 2023-10-02 17:21:07.000000 tweet-capture-0.2.4/tweetcapture/utils/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:07:14.842250 tweet-capture-0.2.5/
+-rw-rw-rw-   0        0        0     1085 2021-05-31 19:56:28.000000 tweet-capture-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     3238 2024-04-15 01:07:14.842991 tweet-capture-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2656 2023-04-06 14:53:44.000000 tweet-capture-0.2.5/README.md
+-rw-rw-rw-   0        0        0       67 2023-04-06 14:53:44.000000 tweet-capture-0.2.5/requirements.txt
+-rw-rw-rw-   0        0        0       86 2024-04-15 01:07:14.844499 tweet-capture-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2024-04-15 00:54:58.000000 tweet-capture-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:07:14.828473 tweet-capture-0.2.5/tweet_capture.egg-info/
+-rw-rw-rw-   0        0        0     3238 2024-04-15 01:07:14.000000 tweet-capture-0.2.5/tweet_capture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2024-04-15 01:07:14.000000 tweet-capture-0.2.5/tweet_capture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 01:07:14.000000 tweet-capture-0.2.5/tweet_capture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-15 01:07:14.000000 tweet-capture-0.2.5/tweet_capture.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       65 2024-04-15 01:07:14.000000 tweet-capture-0.2.5/tweet_capture.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-15 01:07:14.000000 tweet-capture-0.2.5/tweet_capture.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 01:07:14.834715 tweet-capture-0.2.5/tweetcapture/
+-rw-rw-rw-   0        0        0       60 2021-05-31 18:34:46.000000 tweet-capture-0.2.5/tweetcapture/__init__.py
+-rw-rw-rw-   0        0        0     4402 2024-04-15 00:54:58.000000 tweet-capture-0.2.5/tweetcapture/cli.py
+-rw-rw-rw-   0        0        0    18857 2024-04-15 00:54:58.000000 tweet-capture-0.2.5/tweetcapture/screenshot.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:07:14.840739 tweet-capture-0.2.5/tweetcapture/utils/
+-rw-rw-rw-   0        0        0        0 2021-05-31 19:53:06.000000 tweet-capture-0.2.5/tweetcapture/utils/__init__.py
+-rw-rw-rw-   0        0        0     1860 2023-09-22 19:05:50.000000 tweet-capture-0.2.5/tweetcapture/utils/utils.py
+-rw-rw-rw-   0        0        0     2474 2023-10-02 17:21:07.000000 tweet-capture-0.2.5/tweetcapture/utils/webdriver.py
```

### Comparing `tweet-capture-0.2.4/LICENSE` & `tweet-capture-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tweet-capture-0.2.4/PKG-INFO` & `tweet-capture-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweet-capture
-Version: 0.2.4
+Version: 0.2.5
 Summary: Take a tweet screenshot
 Home-page: https://github.com/Xacnio/tweetcapture
 Author: Alperen Çetin
 Author-email: xacnio@pm.me
 License: MIT
 Keywords: tweet screenshot
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `tweet-capture-0.2.4/README.md` & `tweet-capture-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `tweet-capture-0.2.4/setup.py` & `tweet-capture-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     with open('requirements.txt', 'r') as f:
         requirements = f.read().splitlines()
         return requirements
 
 
 setuptools.setup(
     name="tweet-capture",
-    version="0.2.4",
+    version="0.2.5",
     author="Alperen Çetin",
     author_email="xacnio@pm.me",
     description="Take a tweet screenshot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Xacnio/tweetcapture",
     packages=setuptools.find_packages(),
```

### Comparing `tweet-capture-0.2.4/tweet_capture.egg-info/PKG-INFO` & `tweet-capture-0.2.5/tweet_capture.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweet-capture
-Version: 0.2.4
+Version: 0.2.5
 Summary: Take a tweet screenshot
 Home-page: https://github.com/Xacnio/tweetcapture
 Author: Alperen Çetin
 Author-email: xacnio@pm.me
 License: MIT
 Keywords: tweet screenshot
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `tweet-capture-0.2.4/tweetcapture/cli.py` & `tweet-capture-0.2.5/tweetcapture/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     parser.add_argument('-m', "--mode", type=int, help="Mods to show/hide some tweet items (0-4)", default=3)
     parser.add_argument('-t', type=float, help="Waiting time while the page loading (1.0-10.0)", default=5.0)
     parser.add_argument("-n", "--night-mode", type=int, help="Twitter night mode theme (0-2)", default=0)
     parser.add_argument('--lang', type=str,help="Browser language code (tr,en,es,..)", default="")
     parser.add_argument('--chromedriver', type=str, help="Custom chromedriver path", default="")
     parser.add_argument('-o', '--output', type=str, help="Output file name", default="")
     parser.add_argument('-sp', '--show-parent-tweets', dest='show_parent_tweets', action='store_true', help="Show parent tweets")
+    parser.add_argument('-spl', '--show-parent-limit', type=int, help="Show parent tweets limit (default: -1 = unlimited)", default=-1)
     parser.add_argument('-sm', '--show-mentions', type=int, help="Show mentions count (default: 0)", default=0)
     parser.add_argument('-r', '--radius', type=int, help="Image radius", default=15)
     parser.add_argument('-s', '--scale', type=float, help="Screenshot scale (between 0.0 and 14.0) (1.0 = original, 2.0 = 2x high) (default: 1.0)", default=1.0)
 
     parser.add_argument('-hp', '--hide-photos', dest='hide_tweet_photos', action='store_true', help="Hide tweet photos")
     parser.add_argument('-hv', '--hide-videos', dest='hide_tweet_videos', action='store_true', help="Hide tweet videos")
     parser.add_argument('-hg', '--hide-gifs', dest='hide_tweet_gifs', action='store_true', help="Hide tweet gifs")
@@ -24,23 +25,23 @@
     parser.add_argument('-hlp', '--hide-link-previews', dest='hide_tweet_link_previews', action='store_true', help="Hide tweet link previews")
     parser.add_argument('-ha', '--hide-all', dest='hide_all_tweet_medias', action='store_true', help="Hide all tweet medias")
     
     parser.add_argument('--overwrite', dest='overwrite', action='store_true', help="Overwrite output file if exists")
     parser.add_argument('-d', '--debug', dest='debug', action='store_true', help="Debug mode")
     parser.add_argument('--gui', dest='gui', action='store_true', help="GUI mode, open browser window")
     parser.add_argument('--cookies', type=str, help="Set cookies cookie1=value1;cookie2=value2", default="")
-    parser.set_defaults(show_parent_tweets=False, overwrite=False, debug=False, gui=False, hide_tweet_photos=False, hide_tweet_videos=False, hide_tweet_gifs=False, hide_tweet_quotes=False, hide_tweet_link_previews=False, hide_all_tweet_medias=False)
+    parser.set_defaults(show_parent_limit=-1, show_parent_tweets=False, overwrite=False, debug=False, gui=False, hide_tweet_photos=False, hide_tweet_videos=False, hide_tweet_gifs=False, hide_tweet_quotes=False, hide_tweet_link_previews=False, hide_all_tweet_medias=False)
 
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
-    tweet = TweetCapture(args.mode, args.night_mode, show_parent_tweets=args.show_parent_tweets, show_mentions_count=args.show_mentions, overwrite=args.overwrite, radius=args.radius, scale=args.scale)
+    tweet = TweetCapture(args.mode, args.night_mode, show_parent_tweets=args.show_parent_tweets, parent_tweets_limit=args.show_parent_limit, show_mentions_count=args.show_mentions, overwrite=args.overwrite, radius=args.radius, scale=args.scale)
     tweet.set_lang(args.lang)
     tweet.set_wait_time(args.t)
     if args.hide_all_tweet_medias is True: 
         tweet.hide_all_media()
     else: 
         tweet.hide_media(args.hide_tweet_link_previews, args.hide_tweet_photos, args.hide_tweet_videos, args.hide_tweet_gifs, args.hide_tweet_quotes)
     tweet.set_gui(args.gui)
```

### Comparing `tweet-capture-0.2.4/tweetcapture/screenshot.py` & `tweet-capture-0.2.5/tweetcapture/screenshot.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,41 +14,43 @@
     mode = 3
     night_mode = 0
     wait_time = 5
     chrome_opts = []
     lang = None
     test = False
     show_parent_tweets = False
+    parent_tweets_limit = 0
     show_mentions_count = 0
     overwrite = False
     radius = 15
     scale = 1.0
     cookies = None
 
     hide_link_previews = False
     hide_photos = False
     hide_videos = False
     hide_gifs = False
     hide_quotes = False
 
     __web = 1
 
-    def __init__(self, mode=3, night_mode=0, test=False, show_parent_tweets=False, show_mentions_count=0, overwrite=False, radius=15, scale=1.0):
+    def __init__(self, mode=3, night_mode=0, test=False, show_parent_tweets=False, parent_tweets_limit=0, show_mentions_count=0, overwrite=False, radius=15, scale=1.0):
         self.set_night_mode(night_mode)
         self.set_mode(mode)
         self.set_scale(scale)
         self.test = test
         self.show_parent_tweets = show_parent_tweets
+        self.parent_tweets_limit = parent_tweets_limit
         self.show_mentions_count = show_mentions_count
         self.overwrite = overwrite
         self.radius = radius
         if environ.get('AUTH_TOKEN') != None:
             self.cookies = [{'name': 'auth_token', 'value': environ.get('AUTH_TOKEN')}]
 
-    async def screenshot(self, url, path=None, mode=None, night_mode=None, show_parent_tweets=None, show_mentions_count=None, overwrite=None, radius=None, scale=None):
+    async def screenshot(self, url, path=None, mode=None, night_mode=None, show_parent_tweets=None, parent_tweets_limit=None, show_mentions_count=None, overwrite=None, radius=None, scale=None):
         if is_valid_tweet_url(url) is False:
             raise Exception("Invalid tweet url")
 
         if not isinstance(path, str) or len(path) == 0:
             path = get_tweet_file_name(url)
 
         if exists(path):
@@ -80,15 +82,15 @@
             self.__hide_global_items(driver)
             driver.execute_script("!!document.activeElement ? document.activeElement.blur() : 0")
 
             if self.test is True: 
                 driver.save_screenshot(f"web{self.__web}.png")
                 self.__web += 1
             await sleep(2.0)
-            elements, main = self.__get_tweets(driver, self.show_parent_tweets if show_parent_tweets is None else show_parent_tweets, self.show_mentions_count if show_mentions_count is None else show_mentions_count)
+            elements, main = self.__get_tweets(driver, self.show_parent_tweets if show_parent_tweets is None else show_parent_tweets, self.parent_tweets_limit if parent_tweets_limit is None else parent_tweets_limit, self.show_mentions_count if show_mentions_count is None else show_mentions_count)
             if len(elements) == 0:
                 raise Exception("Tweets not found")
             else:
                 for i, element in enumerate(elements):
                     if i == main:
                         self.__code_main_footer_items_new(element, self.mode if mode is None else mode)
                     else:
@@ -367,15 +369,15 @@
         brdr = element.find_elements(By.XPATH, XPATHS[2])
         if len(brdr) == 1:
             element.parent.execute_script("""
             arguments[0].style.borderBottom="none";
             """, brdr[0])
 
     # Return: (elements, main_element_index)
-    def __get_tweets(self, driver, show_parents, show_mentions_count):
+    def __get_tweets(self, driver, show_parents, parent_tweets_limit, show_mentions_count):
         els = driver.find_elements(By.XPATH, "(//ancestor::article)/..")
         elements = []
         for element in els:
             if len(element.find_elements(By.XPATH, ".//article[contains(@data-testid, 'tweet')]")) > 0:
                 source = element.get_attribute("innerHTML")
                 # sponsored tweet pass
                 if source.find("M19.498 3h-15c-1.381 0-2.5 1.12-2.5 2.5v13c0 1.38") != -1 or source.find('css-1dbjc4n r-1s2bzr4" id="id__jrl5cg7nxl"') != -1:
@@ -393,23 +395,26 @@
                         main_element = i
                         break
                 if main_element == -1:
                     return [], -1
                 else:
                     r = main_element+1
                     r2 = r+show_mentions_count
+                    s1 = 0
+                    if parent_tweets_limit > 0 and len(elements[s1:main_element]) > parent_tweets_limit:
+                        s1 = main_element - parent_tweets_limit
                     if show_parents and show_mentions_count > 0:
-                        if len(elements[r:]) > show_mentions_count:                   
-                            return (elements[0:r] + elements[r:r2]), main_element
-                        return elements, main_element
+                        if len(elements[r:]) > show_mentions_count:      
+                            return (elements[s1:r] + elements[r:r2]), main_element
+                        return elements[s1:], main_element
                     elif show_parents:
                         if main_element == 0:
                             return elements[0:1], 0
                         else:
-                            return elements[:r], main_element
+                            return elements[s1:r], main_element
                     elif show_mentions_count > 0:
                         if len(elements[r:]) > show_mentions_count:
                             return elements[main_element:1] + elements[r:r2], 0
                         return elements[main_element:], 0
                     else:
                         return elements[main_element:r], 0
         return [], -1
```

### Comparing `tweet-capture-0.2.4/tweetcapture/utils/utils.py` & `tweet-capture-0.2.5/tweetcapture/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tweet-capture-0.2.4/tweetcapture/utils/webdriver.py` & `tweet-capture-0.2.5/tweetcapture/utils/webdriver.py`

 * *Files identical despite different names*

