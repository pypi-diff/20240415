# Comparing `tmp/livekit_plugins_elevenlabs-0.3.0.tar.gz` & `tmp/livekit-plugins-elevenlabs-0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_plugins_elevenlabs-0.3.0.tar", last modified: Mon Apr 15 20:05:14 2024, max compression
+gzip compressed data, was "livekit-plugins-elevenlabs-0.3.dev0.tar", last modified: Thu Apr 11 22:03:31 2024, max compression
```

## Comparing `livekit_plugins_elevenlabs-0.3.0.tar` & `livekit-plugins-elevenlabs-0.3.dev0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:14.825690 livekit_plugins_elevenlabs-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-15 20:05:14.825690 livekit_plugins_elevenlabs-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-15 20:05:08.000000 livekit_plugins_elevenlabs-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:14.825690 livekit_plugins_elevenlabs-0.3.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:14.825690 livekit_plugins_elevenlabs-0.3.0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:14.825690 livekit_plugins_elevenlabs-0.3.0/livekit/plugins/elevenlabs/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 20:05:08.000000 livekit_plugins_elevenlabs-0.3.0/livekit/plugins/elevenlabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-15 20:05:08.000000 livekit_plugins_elevenlabs-0.3.0/livekit/plugins/elevenlabs/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:08.000000 livekit_plugins_elevenlabs-0.3.0/livekit/plugins/elevenlabs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-04-15 20:05:08.000000 livekit_plugins_elevenlabs-0.3.0/livekit/plugins/elevenlabs/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-15 20:05:08.000000 livekit_plugins_elevenlabs-0.3.0/livekit/plugins/elevenlabs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:05:14.825690 livekit_plugins_elevenlabs-0.3.0/livekit_plugins_elevenlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-15 20:05:14.000000 livekit_plugins_elevenlabs-0.3.0/livekit_plugins_elevenlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-15 20:05:14.000000 livekit_plugins_elevenlabs-0.3.0/livekit_plugins_elevenlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:05:14.000000 livekit_plugins_elevenlabs-0.3.0/livekit_plugins_elevenlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 20:05:14.000000 livekit_plugins_elevenlabs-0.3.0/livekit_plugins_elevenlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 20:05:14.000000 livekit_plugins_elevenlabs-0.3.0/livekit_plugins_elevenlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 20:05:08.000000 livekit_plugins_elevenlabs-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:05:14.825690 livekit_plugins_elevenlabs-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-15 20:05:08.000000 livekit_plugins_elevenlabs-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.950547 livekit-plugins-elevenlabs-0.3.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.950547 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/setup.py
```

### Comparing `livekit_plugins_elevenlabs-0.3.0/PKG-INFO` & `livekit-plugins-elevenlabs-0.3.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-elevenlabs
-Version: 0.3.0
+Version: 0.3.dev0
 Summary: Agent Framework plugin for voice synthesis with ElevenLabs' API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,elevenlabs
```

### Comparing `livekit_plugins_elevenlabs-0.3.0/livekit/plugins/elevenlabs/__init__.py` & `livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_elevenlabs-0.3.0/livekit/plugins/elevenlabs/tts.py` & `livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/tts.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_elevenlabs-0.3.0/livekit/plugins/elevenlabs/version.py` & `livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/version.py`

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

### Comparing `livekit_plugins_elevenlabs-0.3.0/livekit_plugins_elevenlabs.egg-info/PKG-INFO` & `livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-elevenlabs
-Version: 0.3.0
+Version: 0.3.dev0
 Summary: Agent Framework plugin for voice synthesis with ElevenLabs' API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,elevenlabs
```

### Comparing `livekit_plugins_elevenlabs-0.3.0/setup.py` & `livekit-plugins-elevenlabs-0.3.dev0/setup.py`

 * *Files identical despite different names*

