# Comparing `tmp/livekit_plugins_nltk-0.4.0.tar.gz` & `tmp/livekit-plugins-nltk-0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_plugins_nltk-0.4.0.tar", last modified: Mon Apr 15 20:05:20 2024, max compression
+gzip compressed data, was "livekit-plugins-nltk-0.4.dev0.tar", last modified: Thu Apr 11 22:03:41 2024, max compression
```

## Comparing `livekit_plugins_nltk-0.4.0.tar` & `livekit-plugins-nltk-0.4.dev0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:20.058784 livekit_plugins_nltk-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-15 20:05:20.054784 livekit_plugins_nltk-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-15 20:05:16.000000 livekit_plugins_nltk-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:20.054784 livekit_plugins_nltk-0.4.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:20.054784 livekit_plugins_nltk-0.4.0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:20.054784 livekit_plugins_nltk-0.4.0/livekit/plugins/nltk/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-15 20:05:16.000000 livekit_plugins_nltk-0.4.0/livekit/plugins/nltk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:16.000000 livekit_plugins_nltk-0.4.0/livekit/plugins/nltk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-15 20:05:16.000000 livekit_plugins_nltk-0.4.0/livekit/plugins/nltk/sentence_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-15 20:05:16.000000 livekit_plugins_nltk-0.4.0/livekit/plugins/nltk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:20.054784 livekit_plugins_nltk-0.4.0/livekit_plugins_nltk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-15 20:05:20.000000 livekit_plugins_nltk-0.4.0/livekit_plugins_nltk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-15 20:05:20.000000 livekit_plugins_nltk-0.4.0/livekit_plugins_nltk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:05:20.000000 livekit_plugins_nltk-0.4.0/livekit_plugins_nltk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 20:05:20.000000 livekit_plugins_nltk-0.4.0/livekit_plugins_nltk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 20:05:20.000000 livekit_plugins_nltk-0.4.0/livekit_plugins_nltk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 20:05:16.000000 livekit_plugins_nltk-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:05:20.058784 livekit_plugins_nltk-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-15 20:05:16.000000 livekit_plugins_nltk-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.785523 livekit-plugins-nltk-0.4.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-11 22:03:41.785523 livekit-plugins-nltk-0.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.781523 livekit-plugins-nltk-0.4.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.781523 livekit-plugins-nltk-0.4.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.781523 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/sentence_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.785523 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:03:41.785523 livekit-plugins-nltk-0.4.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/setup.py
```

### Comparing `livekit_plugins_nltk-0.4.0/PKG-INFO` & `livekit-plugins-nltk-0.4.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-nltk
-Version: 0.4.0
+Version: 0.4.dev0
 Summary: Agent Framework plugin for NLTK-based text processing.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
```

### Comparing `livekit_plugins_nltk-0.4.0/livekit/plugins/nltk/__init__.py` & `livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_nltk-0.4.0/livekit/plugins/nltk/sentence_tokenizer.py` & `livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_nltk-0.4.0/livekit/plugins/nltk/version.py` & `livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.4.0"
+__version__ = "0.4.dev0"
```

### Comparing `livekit_plugins_nltk-0.4.0/livekit_plugins_nltk.egg-info/PKG-INFO` & `livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-nltk
-Version: 0.4.0
+Version: 0.4.dev0
 Summary: Agent Framework plugin for NLTK-based text processing.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
```

### Comparing `livekit_plugins_nltk-0.4.0/setup.py` & `livekit-plugins-nltk-0.4.dev0/setup.py`

 * *Files identical despite different names*

