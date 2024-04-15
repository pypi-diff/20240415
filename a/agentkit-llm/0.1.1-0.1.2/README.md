# Comparing `tmp/agentkit-llm-0.1.1.tar.gz` & `tmp/agentkit-llm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentkit-llm-0.1.1.tar", last modified: Wed Apr 10 04:00:04 2024, max compression
+gzip compressed data, was "agentkit-llm-0.1.2.tar", last modified: Mon Apr 15 17:41:55 2024, max compression
```

## Comparing `agentkit-llm-0.1.1.tar` & `agentkit-llm-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-10 04:00:04.898106 agentkit-llm-0.1.1/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.1/LICENSE
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     5487 2024-04-10 04:00:04.898106 agentkit-llm-0.1.1/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     5023 2024-04-10 03:25:58.000000 agentkit-llm-0.1.1/README.md
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-04-10 04:00:04.898106 agentkit-llm-0.1.1/setup.cfg
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      929 2024-04-10 04:00:00.000000 agentkit-llm-0.1.1/setup.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-10 04:00:04.894106 agentkit-llm-0.1.1/src/
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-10 04:00:04.894106 agentkit-llm-0.1.1/src/agentkit/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      175 2024-04-08 03:05:03.000000 agentkit-llm-0.1.1/src/agentkit/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      791 2024-04-08 07:51:39.000000 agentkit-llm-0.1.1/src/agentkit/base_afterquery.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     9584 2024-04-08 11:31:16.000000 agentkit-llm-0.1.1/src/agentkit/base_node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.1/src/agentkit/compose_prompt.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.1/src/agentkit/exceptions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.1/src/agentkit/graph.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-10 04:00:04.894106 agentkit-llm-0.1.1/src/agentkit/llm_api/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2661 2024-04-08 11:05:20.000000 agentkit-llm-0.1.1/src/agentkit/llm_api/GPT.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1479 2024-04-08 11:11:53.000000 agentkit-llm-0.1.1/src/agentkit/llm_api/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     3965 2024-04-08 11:05:44.000000 agentkit-llm-0.1.1/src/agentkit/llm_api/base.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     4129 2024-04-08 11:05:36.000000 agentkit-llm-0.1.1/src/agentkit/llm_api/claude.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1403 2024-04-08 11:05:05.000000 agentkit-llm-0.1.1/src/agentkit/llm_api/utils.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2323 2024-04-08 07:54:51.000000 agentkit-llm-0.1.1/src/agentkit/node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.1/src/agentkit/node_functions.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-10 04:00:04.894106 agentkit-llm-0.1.1/src/agentkit_llm.egg-info/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     5487 2024-04-10 04:00:04.000000 agentkit-llm-0.1.1/src/agentkit_llm.egg-info/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      634 2024-04-10 04:00:04.000000 agentkit-llm-0.1.1/src/agentkit_llm.egg-info/SOURCES.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-04-10 04:00:04.000000 agentkit-llm-0.1.1/src/agentkit_llm.egg-info/dependency_links.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-04-10 04:00:04.000000 agentkit-llm-0.1.1/src/agentkit_llm.egg-info/entry_points.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       26 2024-04-10 04:00:04.000000 agentkit-llm-0.1.1/src/agentkit_llm.egg-info/requires.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-04-10 04:00:04.000000 agentkit-llm-0.1.1/src/agentkit_llm.egg-info/top_level.txt
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-15 17:41:55.670139 agentkit-llm-0.1.2/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.2/LICENSE
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     5522 2024-04-15 17:41:55.670139 agentkit-llm-0.1.2/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     5058 2024-04-14 15:43:56.000000 agentkit-llm-0.1.2/README.md
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-04-15 17:41:55.670139 agentkit-llm-0.1.2/setup.cfg
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      929 2024-04-15 17:40:35.000000 agentkit-llm-0.1.2/setup.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-15 17:41:55.670139 agentkit-llm-0.1.2/src/
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-15 17:41:55.670139 agentkit-llm-0.1.2/src/agentkit/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.2/src/agentkit/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2799 2024-04-14 16:35:34.000000 agentkit-llm-0.1.2/src/agentkit/after_query.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-04-14 12:48:55.000000 agentkit-llm-0.1.2/src/agentkit/base_node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.2/src/agentkit/compose_prompt.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.2/src/agentkit/exceptions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.2/src/agentkit/graph.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-15 17:41:55.670139 agentkit-llm-0.1.2/src/agentkit/llm_api/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2661 2024-04-08 11:05:20.000000 agentkit-llm-0.1.2/src/agentkit/llm_api/GPT.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1479 2024-04-08 11:11:53.000000 agentkit-llm-0.1.2/src/agentkit/llm_api/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     3965 2024-04-08 11:05:44.000000 agentkit-llm-0.1.2/src/agentkit/llm_api/base.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4129 2024-04-08 11:05:36.000000 agentkit-llm-0.1.2/src/agentkit/llm_api/claude.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1403 2024-04-08 11:05:05.000000 agentkit-llm-0.1.2/src/agentkit/llm_api/utils.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.2/src/agentkit/node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.2/src/agentkit/node_functions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.2/src/agentkit/utils.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-15 17:41:55.670139 agentkit-llm-0.1.2/src/agentkit_llm.egg-info/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     5522 2024-04-15 17:41:55.000000 agentkit-llm-0.1.2/src/agentkit_llm.egg-info/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      652 2024-04-15 17:41:55.000000 agentkit-llm-0.1.2/src/agentkit_llm.egg-info/SOURCES.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-04-15 17:41:55.000000 agentkit-llm-0.1.2/src/agentkit_llm.egg-info/dependency_links.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-04-15 17:41:55.000000 agentkit-llm-0.1.2/src/agentkit_llm.egg-info/entry_points.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       26 2024-04-15 17:41:55.000000 agentkit-llm-0.1.2/src/agentkit_llm.egg-info/requires.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-04-15 17:41:55.000000 agentkit-llm-0.1.2/src/agentkit_llm.egg-info/top_level.txt
```

### Comparing `agentkit-llm-0.1.1/LICENSE` & `agentkit-llm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.1/PKG-INFO` & `agentkit-llm-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.1
+Version: 0.1.2
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/Holmeswww/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -24,15 +24,15 @@
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI](https://img.shields.io/pypi/v/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI Status](https://pepy.tech/badge/agentkit-llm)](https://pepy.tech/project/agentkit-llm)
 [![Docs](https://readthedocs.org/projects/agentkit/badge/?version=latest)](https://agentkit.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/holmeswww/agentkit)](https://github.com/holmeswww/AgentKit/blob/main/LICENSE)
 ______________________________________________________________________
-![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png)
+![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/teaser.png)
 </div>
 
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="65px"> offers a unified framework for explicitly constructing a complex human "thought process" from simple natural language prompts.
 The user puts together chains of *nodes*, like stacking LEGO pieces. The chains of nodes can be designed to explicitly enforce a naturally *structured* "thought process".
 
 Different arrangements of nodes could represent different functionalities, allowing the user to integrate various functionalities to build multifunctional agents.
 
@@ -45,22 +45,21 @@
 - [Getting Started](#Getting-Started)
 - [Node Components](#Node-Components)
 - [Using AgentKit without Programming Experience](#Using-AgentKit-without-Programming-Experience)
 - [Citing AgnetKit](#Citing-AgentKit)
 
 # Installation
 
-<!-- Installing the AgentKit stable version is as simple as:
+Installing the AgentKit stable version is as simple as:
 
 ```bash
-pip install agentkit
-``` -->
-
+pip install agentkit-llm
+```
 
-To install the cutting edge version from the main branch of this repo, run:
+Otherwise, to install the cutting edge version from the main branch of this repo, run:
 
 ```bash
 git clone https://github.com/holmeswww/AgentKit && cd AgentKit
 pip install -e .
 ```
 
 # Getting Started
@@ -86,15 +85,15 @@
 node2 = BaseNode(subtask2, subtask2, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
 graph.add_node(node2)
 
 subtask3 = "Now, write a full essay on the topic 'LLM Agents for Games'."
 node3 = BaseNode(subtask3, subtask3, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
 graph.add_node(node3)
 
-
+# add dependencies between nodes
 graph.add_edge(subtask1, subtask2)
 graph.add_edge(subtask1, subtask3)
 graph.add_edge(subtask2, subtask3)
 
 result = graph.evaluate() # outputs a dictionary of prompt, answer pairs
 ```
```

### Comparing `agentkit-llm-0.1.1/README.md` & `agentkit-llm-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI](https://img.shields.io/pypi/v/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI Status](https://pepy.tech/badge/agentkit-llm)](https://pepy.tech/project/agentkit-llm)
 [![Docs](https://readthedocs.org/projects/agentkit/badge/?version=latest)](https://agentkit.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/holmeswww/agentkit)](https://github.com/holmeswww/AgentKit/blob/main/LICENSE)
 ______________________________________________________________________
-![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png)
+![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/teaser.png)
 </div>
 
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="65px"> offers a unified framework for explicitly constructing a complex human "thought process" from simple natural language prompts.
 The user puts together chains of *nodes*, like stacking LEGO pieces. The chains of nodes can be designed to explicitly enforce a naturally *structured* "thought process".
 
 Different arrangements of nodes could represent different functionalities, allowing the user to integrate various functionalities to build multifunctional agents.
 
@@ -31,22 +31,21 @@
 - [Getting Started](#Getting-Started)
 - [Node Components](#Node-Components)
 - [Using AgentKit without Programming Experience](#Using-AgentKit-without-Programming-Experience)
 - [Citing AgnetKit](#Citing-AgentKit)
 
 # Installation
 
-<!-- Installing the AgentKit stable version is as simple as:
+Installing the AgentKit stable version is as simple as:
 
 ```bash
-pip install agentkit
-``` -->
-
+pip install agentkit-llm
+```
 
-To install the cutting edge version from the main branch of this repo, run:
+Otherwise, to install the cutting edge version from the main branch of this repo, run:
 
 ```bash
 git clone https://github.com/holmeswww/AgentKit && cd AgentKit
 pip install -e .
 ```
 
 # Getting Started
@@ -72,15 +71,15 @@
 node2 = BaseNode(subtask2, subtask2, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
 graph.add_node(node2)
 
 subtask3 = "Now, write a full essay on the topic 'LLM Agents for Games'."
 node3 = BaseNode(subtask3, subtask3, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
 graph.add_node(node3)
 
-
+# add dependencies between nodes
 graph.add_edge(subtask1, subtask2)
 graph.add_edge(subtask1, subtask3)
 graph.add_edge(subtask2, subtask3)
 
 result = graph.evaluate() # outputs a dictionary of prompt, answer pairs
 ```
```

### Comparing `agentkit-llm-0.1.1/setup.py` & `agentkit-llm-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import pkg_resources
 import pathlib
 
 PKG_NAME = "agentkit-llm"
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 EXTRAS = {
     "logging": ["wandb"],
 }
 
 setuptools.setup(
     name=PKG_NAME,
     version=VERSION,
```

### Comparing `agentkit-llm-0.1.1/src/agentkit/base_node.py` & `agentkit-llm-0.1.2/src/agentkit/base_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .exceptions import AfterQueryError
 from .node_functions import error_msg_default
 from collections.abc import Callable, Awaitable
 from .graph import Graph
-from .base_afterquery import BaseAfterQuery
+from .after_query import BaseAfterQuery
 from .compose_prompt import BaseComposePrompt
 from colorama import Fore, Back, Style
 import copy
 import datetime
 try:
     from wandb.sdk.data_types.trace_tree import Trace
 except:
```

### Comparing `agentkit-llm-0.1.1/src/agentkit/compose_prompt.py` & `agentkit-llm-0.1.2/src/agentkit/compose_prompt.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.1/src/agentkit/exceptions.py` & `agentkit-llm-0.1.2/src/agentkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.1/src/agentkit/graph.py` & `agentkit-llm-0.1.2/src/agentkit/graph.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.1/src/agentkit/llm_api/GPT.py` & `agentkit-llm-0.1.2/src/agentkit/llm_api/GPT.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.1/src/agentkit/llm_api/__init__.py` & `agentkit-llm-0.1.2/src/agentkit/llm_api/__init__.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.1/src/agentkit/llm_api/base.py` & `agentkit-llm-0.1.2/src/agentkit/llm_api/base.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.1/src/agentkit/llm_api/claude.py` & `agentkit-llm-0.1.2/src/agentkit/llm_api/claude.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.1/src/agentkit/llm_api/utils.py` & `agentkit-llm-0.1.2/src/agentkit/llm_api/utils.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.1/src/agentkit/node.py` & `agentkit-llm-0.1.2/src/agentkit/node.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections.abc import Callable, Awaitable
 from .node_functions import error_msg_default
 from .base_node import BaseNode
 from .graph import Graph
 from colorama import Fore, Back, Style
 import typing as t
 
-from .base_afterquery import BaseAfterQuery
+from .after_query import BaseAfterQuery
 from .compose_prompt import ComposePromptDB
 
 class SimpleDBNode(BaseNode):
     """Class for a node in the graph that queries a database.
 
     Each node in the graph is an instance of the SimpleDBNode class. The node is evaluated by querying the LLM with a prompt.
```

### Comparing `agentkit-llm-0.1.1/src/agentkit_llm.egg-info/PKG-INFO` & `agentkit-llm-0.1.2/src/agentkit_llm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.1
+Version: 0.1.2
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/Holmeswww/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -24,15 +24,15 @@
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI](https://img.shields.io/pypi/v/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI Status](https://pepy.tech/badge/agentkit-llm)](https://pepy.tech/project/agentkit-llm)
 [![Docs](https://readthedocs.org/projects/agentkit/badge/?version=latest)](https://agentkit.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/holmeswww/agentkit)](https://github.com/holmeswww/AgentKit/blob/main/LICENSE)
 ______________________________________________________________________
-![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png)
+![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/teaser.png)
 </div>
 
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="65px"> offers a unified framework for explicitly constructing a complex human "thought process" from simple natural language prompts.
 The user puts together chains of *nodes*, like stacking LEGO pieces. The chains of nodes can be designed to explicitly enforce a naturally *structured* "thought process".
 
 Different arrangements of nodes could represent different functionalities, allowing the user to integrate various functionalities to build multifunctional agents.
 
@@ -45,22 +45,21 @@
 - [Getting Started](#Getting-Started)
 - [Node Components](#Node-Components)
 - [Using AgentKit without Programming Experience](#Using-AgentKit-without-Programming-Experience)
 - [Citing AgnetKit](#Citing-AgentKit)
 
 # Installation
 
-<!-- Installing the AgentKit stable version is as simple as:
+Installing the AgentKit stable version is as simple as:
 
 ```bash
-pip install agentkit
-``` -->
-
+pip install agentkit-llm
+```
 
-To install the cutting edge version from the main branch of this repo, run:
+Otherwise, to install the cutting edge version from the main branch of this repo, run:
 
 ```bash
 git clone https://github.com/holmeswww/AgentKit && cd AgentKit
 pip install -e .
 ```
 
 # Getting Started
@@ -86,15 +85,15 @@
 node2 = BaseNode(subtask2, subtask2, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
 graph.add_node(node2)
 
 subtask3 = "Now, write a full essay on the topic 'LLM Agents for Games'."
 node3 = BaseNode(subtask3, subtask3, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
 graph.add_node(node3)
 
-
+# add dependencies between nodes
 graph.add_edge(subtask1, subtask2)
 graph.add_edge(subtask1, subtask3)
 graph.add_edge(subtask2, subtask3)
 
 result = graph.evaluate() # outputs a dictionary of prompt, answer pairs
 ```
```

### Comparing `agentkit-llm-0.1.1/src/agentkit_llm.egg-info/SOURCES.txt` & `agentkit-llm-0.1.2/src/agentkit_llm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 LICENSE
 README.md
 setup.py
 src/agentkit/__init__.py
-src/agentkit/base_afterquery.py
+src/agentkit/after_query.py
 src/agentkit/base_node.py
 src/agentkit/compose_prompt.py
 src/agentkit/exceptions.py
 src/agentkit/graph.py
 src/agentkit/node.py
 src/agentkit/node_functions.py
+src/agentkit/utils.py
 src/agentkit/llm_api/GPT.py
 src/agentkit/llm_api/__init__.py
 src/agentkit/llm_api/base.py
 src/agentkit/llm_api/claude.py
 src/agentkit/llm_api/utils.py
 src/agentkit_llm.egg-info/PKG-INFO
 src/agentkit_llm.egg-info/SOURCES.txt
```

