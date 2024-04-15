# Comparing `tmp/libreppc-0.1.7.tar.gz` & `tmp/libreppc-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreppc-0.1.7.tar", last modified: Mon Apr 15 03:56:20 2024, max compression
+gzip compressed data, was "libreppc-0.1.8.tar", last modified: Mon Apr 15 05:24:22 2024, max compression
```

## Comparing `libreppc-0.1.7.tar` & `libreppc-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 03:56:20.819943 libreppc-0.1.7/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.7/LICENSE
--rw-r--r--   0 warlock   (1000) warlock   (1000)       98 2024-04-15 03:54:05.000000 libreppc-0.1.7/MANIFEST.in
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-15 03:56:20.819943 libreppc-0.1.7/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1500 2024-04-14 17:20:23.000000 libreppc-0.1.7/README.md
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 03:56:20.819943 libreppc-0.1.7/libreppc/
--rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-15 03:55:35.000000 libreppc-0.1.7/libreppc/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      783 2024-04-14 20:43:38.000000 libreppc-0.1.7/libreppc/__main__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     6340 2024-04-14 20:41:05.000000 libreppc-0.1.7/libreppc/libreppc.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 03:56:20.819943 libreppc-0.1.7/libreppc/static/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2736 2024-04-14 20:52:00.000000 libreppc-0.1.7/libreppc/static/bloger.css
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2720 2024-04-14 20:51:42.000000 libreppc-0.1.7/libreppc/static/mastodon.css
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 03:56:20.819943 libreppc-0.1.7/libreppc/templates/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2706 2024-04-14 20:16:12.000000 libreppc-0.1.7/libreppc/templates/index.html
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2693 2024-04-14 20:38:07.000000 libreppc-0.1.7/libreppc/templates/post.html
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 03:56:20.819943 libreppc-0.1.7/libreppc.egg-info/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-15 03:56:20.000000 libreppc-0.1.7/libreppc.egg-info/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)      375 2024-04-15 03:56:20.000000 libreppc-0.1.7/libreppc.egg-info/SOURCES.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-15 03:56:20.000000 libreppc-0.1.7/libreppc.egg-info/dependency_links.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-15 03:56:20.000000 libreppc-0.1.7/libreppc.egg-info/requires.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-15 03:56:20.000000 libreppc-0.1.7/libreppc.egg-info/top_level.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-15 03:56:20.819943 libreppc-0.1.7/setup.cfg
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1101 2024-04-15 03:53:26.000000 libreppc-0.1.7/setup.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 05:24:22.080480 libreppc-0.1.8/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.8/LICENSE
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       98 2024-04-15 03:54:05.000000 libreppc-0.1.8/MANIFEST.in
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-15 05:24:22.080480 libreppc-0.1.8/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1500 2024-04-14 17:20:23.000000 libreppc-0.1.8/README.md
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 05:24:22.080480 libreppc-0.1.8/libreppc/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-15 05:23:55.000000 libreppc-0.1.8/libreppc/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      786 2024-04-15 04:47:48.000000 libreppc-0.1.8/libreppc/__main__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     7253 2024-04-15 04:57:04.000000 libreppc-0.1.8/libreppc/libreppc.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 05:24:22.080480 libreppc-0.1.8/libreppc/static/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     3034 2024-04-15 05:09:28.000000 libreppc-0.1.8/libreppc/static/bloger.css
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2778 2024-04-15 05:22:36.000000 libreppc-0.1.8/libreppc/static/mastodon.css
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 05:24:22.080480 libreppc-0.1.8/libreppc/templates/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2987 2024-04-15 05:04:21.000000 libreppc-0.1.8/libreppc/templates/index.html
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2869 2024-04-15 05:04:41.000000 libreppc-0.1.8/libreppc/templates/post.html
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 05:24:22.080480 libreppc-0.1.8/libreppc.egg-info/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-15 05:24:21.000000 libreppc-0.1.8/libreppc.egg-info/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      375 2024-04-15 05:24:22.000000 libreppc-0.1.8/libreppc.egg-info/SOURCES.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-15 05:24:21.000000 libreppc-0.1.8/libreppc.egg-info/dependency_links.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-15 05:24:21.000000 libreppc-0.1.8/libreppc.egg-info/requires.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-15 05:24:21.000000 libreppc-0.1.8/libreppc.egg-info/top_level.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-15 05:24:22.080480 libreppc-0.1.8/setup.cfg
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1101 2024-04-15 03:53:26.000000 libreppc-0.1.8/setup.py
```

### Comparing `libreppc-0.1.7/LICENSE` & `libreppc-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.7/PKG-INFO` & `libreppc-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `libreppc-0.1.7/README.md` & `libreppc-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.7/libreppc/__main__.py` & `libreppc-0.1.8/libreppc/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 @app.route('/')
 def main_page() -> str:
     return libreppc.render_main()
 
 @app.route('/post/<string:postId>')
 def post_page(postId: str) -> str:
     return libreppc.render_post(
-        libreppc.find_post_file(postId.removesuffix('.html')), 
+        libreppc.find_post_file_id(postId.removesuffix('.html')), 
         postId
     )
 
 @app.route('/feed.atom')
 def feed():
     libreppc.generate_rss().atom_file('feed.atom')
     return send_file('feed.atom', download_name='feed.atom', mimetype='application/atom+xml')
```

### Comparing `libreppc-0.1.7/libreppc/libreppc.py` & `libreppc-0.1.8/libreppc/libreppc.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,66 @@
         self.app = app
         self.data = json.load(open("config.json"))
         self.load_blog_previews()
 
         if not 'theme' in self.data.keys():
             self.data['theme'] = 'mastodon'
 
+    def table_to_json(self, text: str) -> dict:
+        lines = text.split('\n')
+        ret, keys = list(), list()
+        for index, line in enumerate(lines):
+            if index == 0:
+                keys = [_index.strip() for _index in line.split('|')]
+            elif index == 1: continue
+            else:
+                ret.append({keys[_index]:value.strip() for _index, value in enumerate(line.split('|')) if  _index > 0 and _index < len(keys) - 1})
+        return ret[0]
+
+    def parse_post_metadata(self, postId: str) -> dict:
+        file = self.get_post_file(
+            self.find_post_file_id(postId.removesuffix('.md'))
+        )
+        blog_dir = self.data['blog_dir']
+        with open(f'{blog_dir}/{file}.md', 'r') as fl:
+            table = '\n'.join(fl.read().split('\n')[:3])
+            return self.table_to_json(table)
+
+    def remove_post_metadata(self, text: str) -> str:
+        return '\n'.join(text.split('\n')[3:])
+
+    def get_post_files(self) -> list:
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
+    def find_post_file_id(self, postId: str) -> int:
+        for index, file in enumerate(self.get_post_files()):
+            if file.removesuffix('.md') == postId:
+                return index
+        return -1
+
+    def make_post_dict(self, postId: str, html: str) -> dict:
+        cleaner = re.compile('<.*?>')
+        data = self.parse_post_metadata(postId)
+        return {
+            **data,
+            'id' : postId.removesuffix('.md'),
+            'plain_title' : re.sub(cleaner, '', data['title']),
+            'plain_description' : re.sub(cleaner, '', data['description']),
+            'text' : html
+        }
+
     def render_main(self, is_building: bool=False) -> str:
         data = self.data.copy()
         if is_building:
             data['basepath'] = './'
         else:
             data['basepath'] = '../'
 
@@ -39,14 +91,15 @@
 
         text = ""
         blog_dir = self.data['blog_dir']
         postId = postId.replace('.html', '')
         with open(f'{blog_dir}/{postId}.md') as file:
             text = file.read()
 
+        text = self.remove_post_metadata(text)
         html = markdown.markdown(text, extensions=['fenced_code', 'nl2br', 'tables'])
         data = self.data.copy()
         data['post'] = self.make_post_dict(postId, html)
         data['previous_post'] = previous_post
         data['next_post'] = next_post
 
         render = render_template("post.html", **data)
@@ -91,60 +144,28 @@
 
                 updated = datetime.fromtimestamp(os.path.getmtime(path))
                 updated = utc.localize(updated)
                 fe.updated(updated)
 
         return fg
 
-    def make_post_dict(self, postId: str, html: str) -> dict:
-        cleaner = re.compile('<.*?>')
-        lines = html.split('\n')
-        title = lines[0]
-        description = '\n'.join(lines[:3])
-        return {
-            'id' : postId.replace('.md', ''),
-            'title' : title,
-            'description' : description,
-            'plain_title' : re.sub(cleaner, '', title),
-            'plain_description' : re.sub(cleaner, '', description),
-            'text' : html
-        }
-
     def load_blog_previews(self) -> None:
         blog_dir = self.data['blog_dir']
         self.data['blog'] = list()
         for filename in self.get_post_files():
             with open(f"{blog_dir}/{filename}", 'r', encoding="utf-8") as file:
                 text = file.read()
                 html = markdown.markdown(
                     text, 
                     extensions=['fenced_code', 'nl2br', 'tables']
                 )
                 self.data['blog'].append(
                     self.make_post_dict(filename, html)
                 )
 
-    def get_post_files(self) -> list:
-        files = os.listdir(self.data['blog_dir'])
-        files.sort()
-        files.reverse()
-        return files
-
-    def get_post_file(self, index: int) -> str | None:
-        if index < 0: return None
-        files = self.get_post_files()
-        if index >= len(files): return None
-        return self.get_post_files()[index].removesuffix('.md')
-
-    def find_post_file(self, postId: str) -> int:
-        for index, file in enumerate(self.get_post_files()):
-            if file.removesuffix('.md') == postId:
-                return index
-        return -1
-
     def parse_args(self):
         parser = argparse.ArgumentParser(
             prog='LibrePPC',
             description='A simple profile page creator',
         )
         parser.add_argument('-b', '--build', action='store_true')
         parser.add_argument('-s', '--serve', action='store_true')
```

### Comparing `libreppc-0.1.7/libreppc/static/bloger.css` & `libreppc-0.1.8/libreppc/static/bloger.css`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 .profile {
     border-radius: 10px;
     background: #282828;
     float: right;
     width: 30%;
     margin-left: 3%;
+    position: sticky;
+    top: 10px;
 }
 
 .avatar {
     height: 96px;
     border-radius: 50%;
     overflow: hidden;
     display: inline-block;
@@ -106,50 +108,67 @@
 
 /* On mouse-over, add a deeper shadow */
 .project:hover {
 }
 
 .blog {
     padding: 1%;
-    background: #282828;
     display: grid;
     grid-template-columns: repeat(1, 1fr);
     gap: 10px;
     grid-auto-rows: minmax(auto, auto);
 }
 
 .blog a {
     color: #ffffff;
     text-decoration: none;
 }
 
 .post {
     text-align: left;
-    padding: 6px;
+    padding: 12px;
     margin: 4px;
     background: #222222;
-    border: 0px;
+    border-style: solid;
+    border-width: 1px;
+    border-color: #303030;
+    border-radius: 10px;
     min-height: 128px;
     box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
     transition: 0.3s;
 }
 
 .post h1 {
-    text-align: center;
+    margin: 0px;
+    text-align: left;
+    font-size: 25px;
 }
 
 .post:hover {
     box-shadow: 0 8px 16px 0 rgba(0,0,0,0.4);
 }
 
+.post:active {
+    transform: scale(0.85);
+}
+
+.post .description {
+    color: rgb(164, 156, 144);
+}
+
+.metadata p {
+    display: inline;
+    font-size: 14px;
+    color: rgb(164, 156, 144);
+}
+
 .postbody {
     text-align: left;
     padding: 12px;
     margin: 4px;
-    background: #222222;
     border: 0px;
     width: 65%;
 }
 
 .navigation {
     display: grid;
     grid-template-columns: repeat(2, 1fr);
```

### Comparing `libreppc-0.1.7/libreppc/static/mastodon.css` & `libreppc-0.1.8/libreppc/static/mastodon.css`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,19 @@
     text-align: center;
 }
 
 .post:hover {
     box-shadow: 0 8px 16px 0 rgba(0,0,0,0.4);
 }
 
+.metadata p {
+    color: #586884;
+    font-size: 14px;
+}
+
 .postbody {
     background: #1f232b;
     text-align: left;
     padding: 12px;
     margin: 4px;
     border: 0px;
 }
```

### Comparing `libreppc-0.1.7/libreppc/templates/index.html` & `libreppc-0.1.8/libreppc/templates/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -65,15 +65,21 @@
         <div class="blog">
 
             <h1>{{ blog_title }}</h1>
             
             {% for post in blog %}
             <a href="post/{{ post["id"] }}.html">
                 <div class="post">
-                    {{ post["description"] }}
+                    <h1 class="title">{{ post["title"] }}</h1>
+                    <p class="description">
+                        {{ post["description"] }}
+                    </p>
+                    <div class="metadata">
+                        <p>{{ post["date"] }} • {{ post["author"] }}</p>
+                    </div>
                 </div>
             </a>
             {% endfor %}
         </div>
 
     </div>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -17,9 +17,11 @@
 }" target="_blank">
 ******** {{{{ pprroojjeecctt[[""ttiittllee""]] }}}} ********
 {{ project["description"] }}
 {% endfor %}
 ************ {{{{ bblloogg__ttiittllee }}}} ************
 {% for post in blog %}
 }.html">
+************ {{{{ ppoosstt[[""ttiittllee""]] }}}} ************
 {{ post["description"] }}
+{{ post["date"] }} • {{ post["author"] }}
 {% endfor %}
```

### Comparing `libreppc-0.1.7/libreppc/templates/post.html` & `libreppc-0.1.8/libreppc/templates/post.html`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,18 @@
                     {% endif %}
                 </div>
                 {% endfor %}
             </div>
         </div>
 
         <div class="postbody">
+            <h1 class="title">{{ post["title"] }}</h1>
+            <div class="metadata">
+                <p>{{ post["date"] }} • {{ post["author"] }}</p>
+            </div>
             {{ post["text"] }}
         </div>
 
         <div class="navigation">
             {% if previous_post %}
                 <div class="previous-post">
                     <a href="{{ previous_post }}.html">
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -12,13 +12,15 @@
 {% if supporter["type"] == "text" %}
 {{ supporter["title"] }}
 {{ supporter["target"] }} {% else %}
 {{ supporter["title"] }}
 }" target="_blank">{{ supporter["target"] }}
  {% endif %}
 {% endfor %}
+************ {{{{ ppoosstt[[""ttiittllee""]] }}}} ************
+{{ post["date"] }} • {{ post["author"] }}
 {{ post["text"] }}
 {% if previous_post %}
 _P_r_e_v_i_o_u_s_ _p_o_s_t
 {% endif %} {% if next_post %}
 _N_e_x_t_ _p_o_s_t
 {% endif %}
```

### Comparing `libreppc-0.1.7/libreppc.egg-info/PKG-INFO` & `libreppc-0.1.8/libreppc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `libreppc-0.1.7/setup.py` & `libreppc-0.1.8/setup.py`

 * *Files identical despite different names*

