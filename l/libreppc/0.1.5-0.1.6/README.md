# Comparing `tmp/libreppc-0.1.5.tar.gz` & `tmp/libreppc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreppc-0.1.5.tar", last modified: Sun Apr 14 20:05:27 2024, max compression
+gzip compressed data, was "libreppc-0.1.6.tar", last modified: Sun Apr 14 20:52:51 2024, max compression
```

## Comparing `libreppc-0.1.5.tar` & `libreppc-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 20:05:27.192199 libreppc-0.1.5/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.5/LICENSE
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 20:05:27.192199 libreppc-0.1.5/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1500 2024-04-14 17:20:23.000000 libreppc-0.1.5/README.md
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 20:05:27.192199 libreppc-0.1.5/libreppc/
--rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-14 20:04:55.000000 libreppc-0.1.5/libreppc/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      705 2024-04-14 17:18:08.000000 libreppc-0.1.5/libreppc/__main__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     5555 2024-04-14 17:31:16.000000 libreppc-0.1.5/libreppc/libreppc.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 20:05:27.192199 libreppc-0.1.5/libreppc.egg-info/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 20:05:27.000000 libreppc-0.1.5/libreppc.egg-info/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)      248 2024-04-14 20:05:27.000000 libreppc-0.1.5/libreppc.egg-info/SOURCES.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-14 20:05:27.000000 libreppc-0.1.5/libreppc.egg-info/dependency_links.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-14 20:05:27.000000 libreppc-0.1.5/libreppc.egg-info/requires.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-14 20:05:27.000000 libreppc-0.1.5/libreppc.egg-info/top_level.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-14 20:05:27.192199 libreppc-0.1.5/setup.cfg
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1070 2024-04-14 16:02:17.000000 libreppc-0.1.5/setup.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 20:52:51.850504 libreppc-0.1.6/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.6/LICENSE
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 20:52:51.850504 libreppc-0.1.6/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1500 2024-04-14 17:20:23.000000 libreppc-0.1.6/README.md
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 20:52:51.850504 libreppc-0.1.6/libreppc/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-14 20:52:26.000000 libreppc-0.1.6/libreppc/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      783 2024-04-14 20:43:38.000000 libreppc-0.1.6/libreppc/__main__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     6340 2024-04-14 20:41:05.000000 libreppc-0.1.6/libreppc/libreppc.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 20:52:51.850504 libreppc-0.1.6/libreppc.egg-info/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 20:52:51.000000 libreppc-0.1.6/libreppc.egg-info/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      248 2024-04-14 20:52:51.000000 libreppc-0.1.6/libreppc.egg-info/SOURCES.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-14 20:52:51.000000 libreppc-0.1.6/libreppc.egg-info/dependency_links.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-14 20:52:51.000000 libreppc-0.1.6/libreppc.egg-info/requires.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-14 20:52:51.000000 libreppc-0.1.6/libreppc.egg-info/top_level.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-14 20:52:51.850504 libreppc-0.1.6/setup.cfg
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1070 2024-04-14 16:02:17.000000 libreppc-0.1.6/setup.py
```

### Comparing `libreppc-0.1.5/LICENSE` & `libreppc-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.5/PKG-INFO` & `libreppc-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `libreppc-0.1.5/README.md` & `libreppc-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.5/libreppc/__main__.py` & `libreppc-0.1.6/libreppc/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 
 @app.route('/')
 def main_page() -> str:
     return libreppc.render_main()
 
 @app.route('/post/<string:postId>')
 def post_page(postId: str) -> str:
-    return libreppc.render_post(postId)
+    return libreppc.render_post(
+        libreppc.find_post_file(postId.removesuffix('.html')), 
+        postId
+    )
 
 @app.route('/feed.atom')
 def feed():
     libreppc.generate_rss().atom_file('feed.atom')
     return send_file('feed.atom', download_name='feed.atom', mimetype='application/atom+xml')
 
 if __name__ == '__main__':
```

### Comparing `libreppc-0.1.5/libreppc/libreppc.py` & `libreppc-0.1.6/libreppc/libreppc.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,30 +17,41 @@
         self.app = app
         self.data = json.load(open("config.json"))
         self.load_blog_previews()
 
         if not 'theme' in self.data.keys():
             self.data['theme'] = 'mastodon'
 
-    def render_main(self) -> str:
-        render = render_template("index.html", **self.data)
+    def render_main(self, is_building: bool=False) -> str:
+        data = self.data.copy()
+        if is_building:
+            data['basepath'] = './'
+        else:
+            data['basepath'] = '../'
+
+        render = render_template("index.html", **data)
         render = render.replace("&lt;", "<")
         render = render.replace("&gt;", ">")
         return render
 
-    def render_post(self, postId: str) -> str:
+    def render_post(self, index: int, postId: str) -> str:
+        previous_post = self.get_post_file(index+1)
+        next_post = self.get_post_file(index-1)
+
         text = ""
         blog_dir = self.data['blog_dir']
         postId = postId.replace('.html', '')
         with open(f'{blog_dir}/{postId}.md') as file:
             text = file.read()
 
         html = markdown.markdown(text, extensions=['fenced_code', 'nl2br', 'tables'])
         data = self.data.copy()
         data['post'] = self.make_post_dict(postId, html)
+        data['previous_post'] = previous_post
+        data['next_post'] = next_post
 
         render = render_template("post.html", **data)
         render = render.replace("&lt;", "<")
         render = render.replace("&gt;", ">")
         return render
 
     def generate_rss(self) -> FeedGenerator:
@@ -96,31 +107,43 @@
             'plain_title' : re.sub(cleaner, '', title),
             'plain_description' : re.sub(cleaner, '', description),
             'text' : html
         }
 
     def load_blog_previews(self) -> None:
         blog_dir = self.data['blog_dir']
-        files = os.listdir(blog_dir)
         self.data['blog'] = list()
-        files.sort()
-        files.reverse()
-        for filename in files:
+        for filename in self.get_post_files():
             with open(f"{blog_dir}/{filename}", 'r', encoding="utf-8") as file:
                 text = file.read()
                 html = markdown.markdown(
                     text, 
                     extensions=['fenced_code', 'nl2br', 'tables']
                 )
                 self.data['blog'].append(
                     self.make_post_dict(filename, html)
                 )
 
     def get_post_files(self) -> list:
-        return os.listdir('blog')
+        files = os.listdir(self.data['blog_dir'])
+        files.sort()
+        files.reverse()
+        return files
+
+    def get_post_file(self, index: int) -> str | None:
+        if index < 0: return None
+        files = self.get_post_files()
+        if index >= len(files): return None
+        return self.get_post_files()[index].removesuffix('.md')
+
+    def find_post_file(self, postId: str) -> int:
+        for index, file in enumerate(self.get_post_files()):
+            if file.removesuffix('.md') == postId:
+                return index
+        return -1
 
     def parse_args(self):
         parser = argparse.ArgumentParser(
             prog='LibrePPC',
             description='A simple profile page creator',
         )
         parser.add_argument('-b', '--build', action='store_true')
@@ -133,25 +156,22 @@
         print("Make build dir...")
         os.makedirs("build/static", exist_ok=True)
         os.makedirs("build/post", exist_ok=True)
 
         with open("build/index.html", "w") as file:
             print("Render index.html...")
             with self.app.app_context():
-                file.write(self.render_main())
+                file.write(self.render_main(True))
 
-        files = self.get_post_files()
-        files.sort()
-        files.reverse()
-        for postname in files:
+        for index, postname in enumerate(self.get_post_files()):
             print(f"Render {postname}...")
             postId = postname.replace('.md', '')
             with open(f"build/post/{postId}.html", "w") as file:
                 with self.app.app_context():
-                    file.write(self.render_post(postId))
+                    file.write(self.render_post(index, postId))
 
         print("Generate rss...")
         fg = self.generate_rss()
         fg.atom_file("build/static/feed.atom")
 
         print("Copy styles...")
         theme = self.data['theme']
```

### Comparing `libreppc-0.1.5/libreppc.egg-info/PKG-INFO` & `libreppc-0.1.6/libreppc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `libreppc-0.1.5/setup.py` & `libreppc-0.1.6/setup.py`

 * *Files identical despite different names*

