# Comparing `tmp/livekit_plugins_openai-0.3.0.tar.gz` & `tmp/livekit-plugins-openai-0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_plugins_openai-0.3.0.tar", last modified: Mon Apr 15 20:05:24 2024, max compression
+gzip compressed data, was "livekit-plugins-openai-0.3.dev0.tar", last modified: Thu Apr 11 22:03:54 2024, max compression
```

## Comparing `livekit_plugins_openai-0.3.0.tar` & `livekit-plugins-openai-0.3.dev0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:24.208338 livekit_plugins_openai-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-15 20:05:24.208338 livekit_plugins_openai-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-15 20:05:19.000000 livekit_plugins_openai-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:24.204338 livekit_plugins_openai-0.3.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:24.204338 livekit_plugins_openai-0.3.0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:24.208338 livekit_plugins_openai-0.3.0/livekit/plugins/openai/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-15 20:05:19.000000 livekit_plugins_openai-0.3.0/livekit/plugins/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-15 20:05:19.000000 livekit_plugins_openai-0.3.0/livekit/plugins/openai/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 20:05:19.000000 livekit_plugins_openai-0.3.0/livekit/plugins/openai/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-15 20:05:19.000000 livekit_plugins_openai-0.3.0/livekit/plugins/openai/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:19.000000 livekit_plugins_openai-0.3.0/livekit/plugins/openai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-15 20:05:19.000000 livekit_plugins_openai-0.3.0/livekit/plugins/openai/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-15 20:05:19.000000 livekit_plugins_openai-0.3.0/livekit/plugins/openai/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-15 20:05:19.000000 livekit_plugins_openai-0.3.0/livekit/plugins/openai/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:24.208338 livekit_plugins_openai-0.3.0/livekit_plugins_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-15 20:05:24.000000 livekit_plugins_openai-0.3.0/livekit_plugins_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-15 20:05:24.000000 livekit_plugins_openai-0.3.0/livekit_plugins_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:05:24.000000 livekit_plugins_openai-0.3.0/livekit_plugins_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 20:05:24.000000 livekit_plugins_openai-0.3.0/livekit_plugins_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 20:05:24.000000 livekit_plugins_openai-0.3.0/livekit_plugins_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 20:05:19.000000 livekit_plugins_openai-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:05:24.208338 livekit_plugins_openai-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 20:05:19.000000 livekit_plugins_openai-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.473533 livekit-plugins-openai-0.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-11 22:03:54.473533 livekit-plugins-openai-0.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.469533 livekit-plugins-openai-0.3.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.469533 livekit-plugins-openai-0.3.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.469533 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.469533 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:03:54.473533 livekit-plugins-openai-0.3.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/setup.py
```

### Comparing `livekit_plugins_openai-0.3.0/PKG-INFO` & `livekit-plugins-openai-0.3.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-openai
-Version: 0.3.0
+Version: 0.3.dev0
 Summary: Agent Framework plugin for services from OpenAI
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
```

### Comparing `livekit_plugins_openai-0.3.0/livekit/plugins/openai/__init__.py` & `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_openai-0.3.0/livekit/plugins/openai/llm.py` & `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/llm.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_openai-0.3.0/livekit/plugins/openai/models.py` & `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/models.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_openai-0.3.0/livekit/plugins/openai/stt.py` & `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/stt.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_openai-0.3.0/livekit/plugins/openai/tts.py` & `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/tts.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_openai-0.3.0/livekit/plugins/openai/version.py` & `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.0"
+__version__ = "0.3.dev0"
```

### Comparing `livekit_plugins_openai-0.3.0/livekit_plugins_openai.egg-info/PKG-INFO` & `livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-openai
-Version: 0.3.0
+Version: 0.3.dev0
 Summary: Agent Framework plugin for services from OpenAI
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
```

### Comparing `livekit_plugins_openai-0.3.0/livekit_plugins_openai.egg-info/SOURCES.txt` & `livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livekit_plugins_openai-0.3.0/setup.py` & `livekit-plugins-openai-0.3.dev0/setup.py`

 * *Files identical despite different names*

