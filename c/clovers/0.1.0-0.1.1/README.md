# Comparing `tmp/clovers-0.1.0.tar.gz` & `tmp/clovers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers-0.1.0.tar", max compression
+gzip compressed data, was "clovers-0.1.1.tar", max compression
```

## Comparing `clovers-0.1.0.tar` & `clovers-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-04-15 03:08:16.293727 clovers-0.1.0/clovers/__init__.py
--rw-r--r--   0        0        0     3748 2024-04-15 06:14:05.759745 clovers-0.1.0/clovers/core/adapter.py
--rw-r--r--   0        0        0      582 2024-04-15 03:01:44.120813 clovers-0.1.0/clovers/core/config.py
--rw-r--r--   0        0        0     6393 2024-04-15 03:02:38.391272 clovers-0.1.0/clovers/core/plugin.py
--rw-r--r--   0        0        0     2774 2024-04-15 02:23:00.885679 clovers-0.1.0/clovers/utils/library.py
--rw-r--r--   0        0        0    10961 2024-04-15 02:23:00.886680 clovers-0.1.0/clovers/utils/linecard.py
--rw-r--r--   0        0        0     1884 2024-04-15 02:23:00.887179 clovers-0.1.0/clovers/utils/tools.py
--rw-r--r--   0        0        0     1086 2024-04-15 03:18:25.255783 clovers-0.1.0/LICENSE
--rw-r--r--   0        0        0      293 2024-04-15 03:01:54.745599 clovers-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9681 2024-04-15 06:29:12.523168 clovers-0.1.0/README.md
--rw-r--r--   0        0        0     9579 1970-01-01 00:00:00.000000 clovers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 03:08:16.293727 clovers-0.1.1/clovers/__init__.py
+-rw-r--r--   0        0        0     3748 2024-04-15 06:14:05.759745 clovers-0.1.1/clovers/core/adapter.py
+-rw-r--r--   0        0        0      582 2024-04-15 03:01:44.120813 clovers-0.1.1/clovers/core/config.py
+-rw-r--r--   0        0        0     6393 2024-04-15 08:29:41.742919 clovers-0.1.1/clovers/core/plugin.py
+-rw-r--r--   0        0        0     2774 2024-04-15 02:23:00.885679 clovers-0.1.1/clovers/utils/library.py
+-rw-r--r--   0        0        0    10961 2024-04-15 08:45:36.432996 clovers-0.1.1/clovers/utils/linecard.py
+-rw-r--r--   0        0        0     1884 2024-04-15 08:48:00.582248 clovers-0.1.1/clovers/utils/tools.py
+-rw-r--r--   0        0        0     1086 2024-04-15 03:18:25.255783 clovers-0.1.1/LICENSE
+-rw-r--r--   0        0        0      645 2024-04-15 08:50:09.136155 clovers-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9681 2024-04-15 06:29:12.523168 clovers-0.1.1/README.md
+-rw-r--r--   0        0        0     9936 1970-01-01 00:00:00.000000 clovers-0.1.1/PKG-INFO
```

### Comparing `clovers-0.1.0/clovers/core/adapter.py` & `clovers-0.1.1/clovers/core/adapter.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.0/clovers/core/config.py` & `clovers-0.1.1/clovers/core/config.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.0/clovers/core/plugin.py` & `clovers-0.1.1/clovers/core/plugin.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.0/clovers/utils/library.py` & `clovers-0.1.1/clovers/utils/library.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.0/clovers/utils/linecard.py` & `clovers-0.1.1/clovers/utils/linecard.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.0/clovers/utils/tools.py` & `clovers-0.1.1/clovers/utils/tools.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.0/LICENSE` & `clovers-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers-0.1.0/README.md` & `clovers-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `clovers-0.1.0/PKG-INFO` & `clovers-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 Metadata-Version: 2.1
 Name: clovers
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
+Provides-Extra: linecard
+Provides-Extra: tools
+Requires-Dist: fonttools (>=4.51.0,<5.0.0) ; extra == "linecard"
+Requires-Dist: httpx (>=0.27.0,<0.28.0) ; extra == "tools"
+Requires-Dist: matplotlib (>=3.8.4,<4.0.0) ; extra == "linecard"
+Requires-Dist: numpy (>=1.26.4,<2.0.0) ; extra == "tools"
+Requires-Dist: pillow (>=10.3.0,<11.0.0) ; extra == "linecard"
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # CLOVERS
 
 _✨ 自定义的聊天平台异步机器人指令-响应插件框架 ✨_
```

