# Comparing `tmp/nonebug-0.3.6.tar.gz` & `tmp/nonebug-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebug-0.3.6.tar", max compression
+gzip compressed data, was "nonebug-0.3.7.tar", max compression
```

## Comparing `nonebug-0.3.6.tar` & `nonebug-0.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2024-03-10 03:45:43.774830 nonebug-0.3.6/LICENSE
--rw-r--r--   0        0        0     1966 2024-03-10 03:45:43.774830 nonebug-0.3.6/README.md
--rw-r--r--   0        0        0      130 2024-03-10 03:45:43.774830 nonebug-0.3.6/nonebug/__init__.py
--rw-r--r--   0        0        0      149 2024-03-10 03:45:43.774830 nonebug-0.3.6/nonebug/app.py
--rw-r--r--   0        0        0     1176 2024-03-10 03:45:43.774830 nonebug-0.3.6/nonebug/base.py
--rw-r--r--   0        0        0      706 2024-03-10 03:45:43.774830 nonebug-0.3.6/nonebug/fixture.py
--rw-r--r--   0        0        0      204 2024-03-10 03:45:43.774830 nonebug-0.3.6/nonebug/mixin/__init__.py
--rw-r--r--   0        0        0     7880 2024-03-10 03:45:43.774830 nonebug-0.3.6/nonebug/mixin/call_api/__init__.py
--rw-r--r--   0        0        0     1655 2024-03-10 03:45:43.774830 nonebug-0.3.6/nonebug/mixin/call_api/fake.py
--rw-r--r--   0        0        0      583 2024-03-10 03:45:43.774830 nonebug-0.3.6/nonebug/mixin/call_api/model.py
--rw-r--r--   0        0        0     1876 2024-03-10 03:45:43.774830 nonebug-0.3.6/nonebug/mixin/dependent.py
--rw-r--r--   0        0        0     1315 2024-03-10 03:45:43.774830 nonebug-0.3.6/nonebug/mixin/driver.py
--rw-r--r--   0        0        0    11198 2024-03-10 03:45:43.774830 nonebug-0.3.6/nonebug/mixin/process/__init__.py
--rw-r--r--   0        0        0     2783 2024-03-10 03:45:43.774830 nonebug-0.3.6/nonebug/mixin/process/fake.py
--rw-r--r--   0        0        0     1314 2024-03-10 03:45:43.774830 nonebug-0.3.6/nonebug/mixin/process/model.py
--rw-r--r--   0        0        0     2908 2024-03-10 03:45:43.774830 nonebug-0.3.6/nonebug/provider.py
--rw-r--r--   0        0        0     2097 2024-03-10 03:45:43.774830 nonebug-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 nonebug-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-15 13:38:35.205196 nonebug-0.3.7/LICENSE
+-rw-r--r--   0        0        0     1966 2024-04-15 13:38:35.205196 nonebug-0.3.7/README.md
+-rw-r--r--   0        0        0      130 2024-04-15 13:38:35.205196 nonebug-0.3.7/nonebug/__init__.py
+-rw-r--r--   0        0        0      149 2024-04-15 13:38:35.205196 nonebug-0.3.7/nonebug/app.py
+-rw-r--r--   0        0        0     1176 2024-04-15 13:38:35.205196 nonebug-0.3.7/nonebug/base.py
+-rw-r--r--   0        0        0      706 2024-04-15 13:38:35.205196 nonebug-0.3.7/nonebug/fixture.py
+-rw-r--r--   0        0        0      204 2024-04-15 13:38:35.205196 nonebug-0.3.7/nonebug/mixin/__init__.py
+-rw-r--r--   0        0        0     7889 2024-04-15 13:38:35.205196 nonebug-0.3.7/nonebug/mixin/call_api/__init__.py
+-rw-r--r--   0        0        0     1655 2024-04-15 13:38:35.205196 nonebug-0.3.7/nonebug/mixin/call_api/fake.py
+-rw-r--r--   0        0        0      583 2024-04-15 13:38:35.205196 nonebug-0.3.7/nonebug/mixin/call_api/model.py
+-rw-r--r--   0        0        0     1876 2024-04-15 13:38:35.205196 nonebug-0.3.7/nonebug/mixin/dependent.py
+-rw-r--r--   0        0        0     1315 2024-04-15 13:38:35.209196 nonebug-0.3.7/nonebug/mixin/driver.py
+-rw-r--r--   0        0        0    11198 2024-04-15 13:38:35.209196 nonebug-0.3.7/nonebug/mixin/process/__init__.py
+-rw-r--r--   0        0        0     2783 2024-04-15 13:38:35.209196 nonebug-0.3.7/nonebug/mixin/process/fake.py
+-rw-r--r--   0        0        0     1314 2024-04-15 13:38:35.209196 nonebug-0.3.7/nonebug/mixin/process/model.py
+-rw-r--r--   0        0        0     2908 2024-04-15 13:38:35.209196 nonebug-0.3.7/nonebug/provider.py
+-rw-r--r--   0        0        0     2097 2024-04-15 13:38:35.209196 nonebug-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 nonebug-0.3.7/PKG-INFO
```

### Comparing `nonebug-0.3.6/LICENSE` & `nonebug-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.6/README.md` & `nonebug-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.6/nonebug/base.py` & `nonebug-0.3.7/nonebug/base.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.6/nonebug/fixture.py` & `nonebug-0.3.7/nonebug/fixture.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.6/nonebug/mixin/call_api/__init__.py` & `nonebug-0.3.7/nonebug/mixin/call_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     Union,
     TypeVar,
     Optional,
     overload,
 )
 
 import pytest
-from nonebot.compat import model_dump
 
 from nonebug.base import BaseApp, Context
 
 from .model import Api, Send, Model
 from .fake import make_fake_bot, make_fake_adapter
 
 if TYPE_CHECKING:
@@ -185,14 +184,16 @@
     def got_call_send(
         self,
         bot: "Bot",
         event: "Event",
         message: Union[str, "Message", "MessageSegment"],
         **kwargs: Any,
     ) -> Any:
+        from nonebot.compat import model_dump
+
         if self.wait_list.empty():
             pytest.fail(
                 "Application has no send call but expected "
                 f"event={event} message={message} kwargs={kwargs}"
             )
         model = self.wait_list.get()
         if not isinstance(model, Send):
```

### Comparing `nonebug-0.3.6/nonebug/mixin/call_api/fake.py` & `nonebug-0.3.7/nonebug/mixin/call_api/fake.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.6/nonebug/mixin/call_api/model.py` & `nonebug-0.3.7/nonebug/mixin/call_api/model.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.6/nonebug/mixin/dependent.py` & `nonebug-0.3.7/nonebug/mixin/dependent.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.6/nonebug/mixin/driver.py` & `nonebug-0.3.7/nonebug/mixin/driver.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.6/nonebug/mixin/process/__init__.py` & `nonebug-0.3.7/nonebug/mixin/process/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.6/nonebug/mixin/process/fake.py` & `nonebug-0.3.7/nonebug/mixin/process/fake.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.6/nonebug/mixin/process/model.py` & `nonebug-0.3.7/nonebug/mixin/process/model.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.6/nonebug/provider.py` & `nonebug-0.3.7/nonebug/provider.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.6/pyproject.toml` & `nonebug-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebug"
-version = "0.3.6"
+version = "0.3.7"
 description = "nonebot2 test framework"
 authors = ["AkiraXie <l997460364@outlook.com>", "yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://nonebot.dev/"
 repository = "https://github.com/nonebot/nonebug"
 documentation = "https://nonebot.dev/"
```

### Comparing `nonebug-0.3.6/PKG-INFO` & `nonebug-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebug
-Version: 0.3.6
+Version: 0.3.7
 Summary: nonebot2 test framework
 Home-page: https://nonebot.dev/
 License: MIT
 Keywords: nonebot,pytest,test,bot,onebot,cqhttp
 Author: AkiraXie
 Author-email: l997460364@outlook.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebug Version: 0.3.6 Summary: nonebot2 test
+Metadata-Version: 2.1 Name: nonebug Version: 0.3.7 Summary: nonebot2 test
 framework Home-page: https://nonebot.dev/ License: MIT Keywords:
 nonebot,pytest,test,bot,onebot,cqhttp Author: AkiraXie Author-email:
 l997460364@outlook.com Requires-Python: >=3.8,<4.0 Classifier: Framework ::
 Pytest Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

