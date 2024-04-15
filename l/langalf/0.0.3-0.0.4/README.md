# Comparing `tmp/langalf-0.0.3.tar.gz` & `tmp/langalf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langalf-0.0.3.tar", max compression
+gzip compressed data, was "langalf-0.0.4.tar", max compression
```

## Comparing `langalf-0.0.3.tar` & `langalf-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11367 2024-04-13 15:29:08.921278 langalf-0.0.3/LICENSE
--rw-r--r--   0        0        0     9036 2024-04-13 15:29:08.921278 langalf-0.0.3/Readme.md
--rw-r--r--   0        0        0        0 2024-04-13 15:29:08.921278 langalf-0.0.3/langalf/__init__.py
--rw-r--r--   0        0        0      429 2024-04-13 15:29:08.921278 langalf-0.0.3/langalf/__main__.py
--rw-r--r--   0        0        0     3522 2024-04-13 15:29:08.921278 langalf-0.0.3/langalf/app.py
--rw-r--r--   0        0        0     2234 2024-04-13 15:29:08.921278 langalf-0.0.3/langalf/http_spec.py
--rw-r--r--   0        0        0        0 2024-04-13 15:29:08.921278 langalf-0.0.3/langalf/probe_actor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 15:29:08.921278 langalf-0.0.3/langalf/probe_actor/__main__.py
--rw-r--r--   0        0        0     3315 2024-04-13 15:29:08.921278 langalf-0.0.3/langalf/probe_actor/fuzzer.py
--rw-r--r--   0        0        0     1180 2024-04-13 15:29:08.921278 langalf-0.0.3/langalf/probe_actor/refusal.py
--rw-r--r--   0        0        0      449 2024-04-13 15:29:08.921278 langalf-0.0.3/langalf/probe_actor/test_refusal.py
--rw-r--r--   0        0        0     3591 2024-04-13 15:29:08.921278 langalf-0.0.3/langalf/probe_data/__init__.py
--rw-r--r--   0        0        0     8416 2024-04-13 15:29:08.921278 langalf-0.0.3/langalf/probe_data/data.py
--rw-r--r--   0        0        0     2645 2024-04-13 15:29:08.921278 langalf-0.0.3/langalf/probe_data/stenography_fn.py
--rw-r--r--   0        0        0    26019 2024-04-13 15:29:08.921278 langalf-0.0.3/langalf/static/index.html
--rw-r--r--   0        0        0     1952 2024-04-13 15:29:08.921278 langalf-0.0.3/langalf/test_spec.py
--rw-r--r--   0        0        0     1122 2024-04-13 15:29:08.921278 langalf-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    10273 1970-01-01 00:00:00.000000 langalf-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11367 2024-04-15 12:40:06.466012 langalf-0.0.4/LICENSE
+-rw-r--r--   0        0        0     9044 2024-04-15 12:40:06.466012 langalf-0.0.4/Readme.md
+-rw-r--r--   0        0        0        0 2024-04-15 12:40:06.466012 langalf-0.0.4/langalf/__init__.py
+-rw-r--r--   0        0        0      429 2024-04-15 12:40:06.466012 langalf-0.0.4/langalf/__main__.py
+-rw-r--r--   0        0        0     3522 2024-04-15 12:40:06.466012 langalf-0.0.4/langalf/app.py
+-rw-r--r--   0        0        0     2234 2024-04-15 12:40:06.466012 langalf-0.0.4/langalf/http_spec.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:40:06.466012 langalf-0.0.4/langalf/probe_actor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:40:06.470012 langalf-0.0.4/langalf/probe_actor/__main__.py
+-rw-r--r--   0        0        0     3315 2024-04-15 12:40:06.470012 langalf-0.0.4/langalf/probe_actor/fuzzer.py
+-rw-r--r--   0        0        0     1180 2024-04-15 12:40:06.470012 langalf-0.0.4/langalf/probe_actor/refusal.py
+-rw-r--r--   0        0        0      449 2024-04-15 12:40:06.470012 langalf-0.0.4/langalf/probe_actor/test_refusal.py
+-rw-r--r--   0        0        0     3591 2024-04-15 12:40:06.470012 langalf-0.0.4/langalf/probe_data/__init__.py
+-rw-r--r--   0        0        0     8416 2024-04-15 12:40:06.470012 langalf-0.0.4/langalf/probe_data/data.py
+-rw-r--r--   0        0        0     2645 2024-04-15 12:40:06.470012 langalf-0.0.4/langalf/probe_data/stenography_fn.py
+-rw-r--r--   0        0        0    26019 2024-04-15 12:40:06.470012 langalf-0.0.4/langalf/static/index.html
+-rw-r--r--   0        0        0     1952 2024-04-15 12:40:06.470012 langalf-0.0.4/langalf/test_spec.py
+-rw-r--r--   0        0        0     1150 2024-04-15 12:40:06.470012 langalf-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    10281 1970-01-01 00:00:00.000000 langalf-0.0.4/PKG-INFO
```

### Comparing `langalf-0.0.3/LICENSE` & `langalf-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langalf-0.0.3/Readme.md` & `langalf-0.0.4/Readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 ```
 ## Probe endpoint
 
 In the example of custom integration, we use `/v1/self-probe` for the sake of integration testing.
 
 
 ```python
-POST https://landalf.vercel.app/v1/self-probe
+POST https://langalf-preview.vercel.app/v1/self-probe
 Authorization: Bearer XXXXX
 Content-Type: application/json
 
 {
     "prompt": "<<PROMPT>>"
 }
 
@@ -276,8 +276,8 @@
 
 <a href="https://cal.com/alexander-myasoedov-go2tfs/30min"><img src="https://cal.com/book-with-cal-dark.svg" alt="Book us with Cal.com"></a>
 
 Book a 1-on-1 Session with the founders, to discuss any issues, provide feedback, or explore how we can improve langalf for you.
 
 ## Repo Activity
 
-<img width="100%" src="https://repobeats.axiom.co/api/embed/6bfca2f20f39738048b6e70ca205efde46352c3d.svg" />
+<img width="100%" src="https://repobeats.axiom.co/api/embed/2b4b4e080d21ef9174ca69bcd801145a71f67aaf.svg" />
```

### Comparing `langalf-0.0.3/langalf/app.py` & `langalf-0.0.4/langalf/app.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.3/langalf/http_spec.py` & `langalf-0.0.4/langalf/http_spec.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.3/langalf/probe_actor/fuzzer.py` & `langalf-0.0.4/langalf/probe_actor/fuzzer.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.3/langalf/probe_actor/refusal.py` & `langalf-0.0.4/langalf/probe_actor/refusal.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.3/langalf/probe_data/__init__.py` & `langalf-0.0.4/langalf/probe_data/__init__.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.3/langalf/probe_data/data.py` & `langalf-0.0.4/langalf/probe_data/data.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.3/langalf/probe_data/stenography_fn.py` & `langalf-0.0.4/langalf/probe_data/stenography_fn.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.3/langalf/static/index.html` & `langalf-0.0.4/langalf/static/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     </script>
   </head>
   <body class="bg-soft p-8">
     <!-- Vue app root element -->
     <div id="vue-app">
       <h4
         class="-mx-20 px-24 text-center bg-earthy-zen py-4 text-l text-white text-dark-primary ">🚀
-        NEW: Star Landalf on <a
+        NEW: Star Langalf on <a
           href="https://github.com/msoedov/langalf"
           target="_blank"
           class="text-dark-primary underline"
           data-faitracker-click-bind="true">Github</a> 🚀</h4>
       <div
         class="header flex items-center justify-between px-4 py-3 text-earth-1 bg-background ">
         <div class="header__title flex items-center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-****** ?🚀 NNEEWW:: SSttaarr LLaannddaallff oonn _GG_ii_tt_hh_uu_bb ?🚀 ******
+****** ?🚀 NNEEWW:: SSttaarr LLaannggaallff oonn _GG_ii_tt_hh_uu_bb ?🚀 ******
 _D_o_c_s
 ******** AAggeennttiicc LLLLMM VVuullnneerraabbiilliittyy SSccaannnneerr [[BBeettaa]] ********
 Input the API LLM spec and specify the maximum budget in tokens.
 Select a config
 key="index" @click="selectConfig(index)" class="border-2 rounded-lg p-4 flex
 flex-col items-start transition-all hover:shadow-md" :class="{'border-earth-1':
 selectedConfig === index, 'border-gray-300': selectedConfig !== index}">
```

### Comparing `langalf-0.0.3/langalf/test_spec.py` & `langalf-0.0.4/langalf/test_spec.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.3/pyproject.toml` & `langalf-0.0.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langalf"
-version = "0.0.3"
+version = "0.0.4"
 description = "Agentic LLM vulnerability scanner"
 authors = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 maintainers = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 repository = "https://github.com/msoedov/langalf"
 license = "MIT"
 readme = "Readme.md"
 keywords = [
@@ -22,27 +22,27 @@
 
 
 [tool.poetry.scripts]
 langalf = "langalf.__main__:entrypoint"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-fastapi = "^0.109.1"
+fastapi = ">=0.109.1,<0.111.0"
 uvicorn = "^0.23.2"
 fire = "^0.5.0"
 loguru = "^0.7.2"
-httpx = "^0.25.1"
+httpx = ">=0.25.1,<0.28.0"
 cache-to-disk = "^2.0.0"
 pandas = "^1.4.0"
 datasets = "^1.14.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.10.1"
 mypy = "^1.6.1"
-httpx = "^0.25.1"
+httpx = ">=0.25.1,<0.28.0"
 pytest = "^7.4.3"
 pre-commit = "^3.5.0"
 
 [tool.ruff]
 line-length = 120
 
 [build-system]
```

### Comparing `langalf-0.0.3/PKG-INFO` & `langalf-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langalf
-Version: 0.0.3
+Version: 0.0.4
 Summary: Agentic LLM vulnerability scanner
 Home-page: https://github.com/msoedov/langalf
 License: MIT
 Keywords: LLM vulnerability scanner,llm security,llm adversarial attacks,prompt injection,prompt leakage,prompt injection attacks,prompt leakage prevention,llm vulnerabilities,owasp-llm-top-10
 Author: Alexander Miasoiedov
 Author-email: msoedov@gmail.com
 Maintainer: Alexander Miasoiedov
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cache-to-disk (>=2.0.0,<3.0.0)
 Requires-Dist: datasets (>=1.14.0,<2.0.0)
-Requires-Dist: fastapi (>=0.109.1,<0.110.0)
+Requires-Dist: fastapi (>=0.109.1,<0.111.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
-Requires-Dist: httpx (>=0.25.1,<0.26.0)
+Requires-Dist: httpx (>=0.25.1,<0.28.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pandas (>=1.4.0,<2.0.0)
 Requires-Dist: uvicorn (>=0.23.2,<0.24.0)
 Project-URL: Repository, https://github.com/msoedov/langalf
 Description-Content-Type: text/markdown
 
 <p align="center">
@@ -225,15 +225,15 @@
 ```
 ## Probe endpoint
 
 In the example of custom integration, we use `/v1/self-probe` for the sake of integration testing.
 
 
 ```python
-POST https://landalf.vercel.app/v1/self-probe
+POST https://langalf-preview.vercel.app/v1/self-probe
 Authorization: Bearer XXXXX
 Content-Type: application/json
 
 {
     "prompt": "<<PROMPT>>"
 }
 
@@ -305,9 +305,9 @@
 
 <a href="https://cal.com/alexander-myasoedov-go2tfs/30min"><img src="https://cal.com/book-with-cal-dark.svg" alt="Book us with Cal.com"></a>
 
 Book a 1-on-1 Session with the founders, to discuss any issues, provide feedback, or explore how we can improve langalf for you.
 
 ## Repo Activity
 
-<img width="100%" src="https://repobeats.axiom.co/api/embed/6bfca2f20f39738048b6e70ca205efde46352c3d.svg" />
+<img width="100%" src="https://repobeats.axiom.co/api/embed/2b4b4e080d21ef9174ca69bcd801145a71f67aaf.svg" />
```

