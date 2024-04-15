# Comparing `tmp/gentccode-0.2.6.tar.gz` & `tmp/gentccode-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentccode-0.2.6.tar", max compression
+gzip compressed data, was "gentccode-0.2.7.tar", max compression
```

## Comparing `gentccode-0.2.6.tar` & `gentccode-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-09-13 07:38:48.461356 gentccode-0.2.6/LICENSE
--rw-r--r--   0        0        0     1084 2024-04-10 07:58:28.662833 gentccode-0.2.6/README.md
--rw-r--r--   0        0        0        0 2023-09-08 11:07:44.041027 gentccode-0.2.6/gentccode/__init__.py
--rw-r--r--   0        0        0     1487 2023-09-08 11:12:45.187569 gentccode-0.2.6/gentccode/cartesian_for_case.py
--rw-r--r--   0        0        0     1216 2023-10-24 06:33:03.360847 gentccode-0.2.6/gentccode/check_version.py
--rw-r--r--   0        0        0     3348 2024-04-10 07:48:10.190075 gentccode-0.2.6/gentccode/cli.py
--rw-r--r--   0        0        0    21552 2024-04-10 07:57:26.821826 gentccode-0.2.6/gentccode/convert_to_jmx.py
--rw-r--r--   0        0        0     4311 2023-11-13 08:42:54.613204 gentccode-0.2.6/gentccode/convert_to_locust.py
--rw-r--r--   0        0        0    17994 2023-09-26 08:23:03.100251 gentccode-0.2.6/gentccode/generate_case_code.py
--rw-r--r--   0        0        0     5311 2023-09-11 02:27:59.106915 gentccode-0.2.6/gentccode/merge_api.py
--rw-r--r--   0        0        0     2857 2023-09-15 06:07:23.156642 gentccode-0.2.6/gentccode/produce_search_case.py
--rw-r--r--   0        0        0     7089 2023-09-15 03:39:56.738346 gentccode-0.2.6/gentccode/produce_test_case.py
--rw-r--r--   0        0        0      790 2023-09-13 03:50:15.782471 gentccode-0.2.6/gentccode/read_swagger_rule.py
--rw-r--r--   0        0        0      612 2024-04-12 10:16:32.869965 gentccode-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 gentccode-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-09-13 07:38:48.461356 gentccode-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1084 2024-04-10 07:58:28.662833 gentccode-0.2.7/README.md
+-rw-r--r--   0        0        0      667 2024-04-15 06:48:54.046409 gentccode-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-08 11:07:44.041027 gentccode-0.2.7/src/gentccode/__init__.py
+-rw-r--r--   0        0        0     1487 2023-09-08 11:12:45.187569 gentccode-0.2.7/src/gentccode/cartesian_for_case.py
+-rw-r--r--   0        0        0     1379 2024-04-15 06:47:35.477620 gentccode-0.2.7/src/gentccode/check_version.py
+-rw-r--r--   0        0        0     3348 2024-04-10 07:48:10.190075 gentccode-0.2.7/src/gentccode/cli.py
+-rw-r--r--   0        0        0    21552 2024-04-10 07:57:26.821826 gentccode-0.2.7/src/gentccode/convert_to_jmx.py
+-rw-r--r--   0        0        0     4311 2023-11-13 08:42:54.613204 gentccode-0.2.7/src/gentccode/convert_to_locust.py
+-rw-r--r--   0        0        0    18060 2024-04-15 04:00:35.792867 gentccode-0.2.7/src/gentccode/generate_case_code.py
+-rw-r--r--   0        0        0     5311 2023-09-11 02:27:59.106915 gentccode-0.2.7/src/gentccode/merge_api.py
+-rw-r--r--   0        0        0     2857 2023-09-15 06:07:23.156642 gentccode-0.2.7/src/gentccode/produce_search_case.py
+-rw-r--r--   0        0        0     7089 2023-09-15 03:39:56.738346 gentccode-0.2.7/src/gentccode/produce_test_case.py
+-rw-r--r--   0        0        0      790 2023-09-13 03:50:15.782471 gentccode-0.2.7/src/gentccode/read_swagger_rule.py
+-rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 gentccode-0.2.7/PKG-INFO
```

### Comparing `gentccode-0.2.6/LICENSE` & `gentccode-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.6/README.md` & `gentccode-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.6/gentccode/cartesian_for_case.py` & `gentccode-0.2.7/src/gentccode/cartesian_for_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.6/gentccode/check_version.py` & `gentccode-0.2.7/src/gentccode/check_version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import xmlrpc.client
-import pkg_resources
+# import pkg_resources
+import importlib.metadata
 
 
 def get_latest_version(package_name):
     try:
         client = xmlrpc.client.ServerProxy("https://pypi.org/pypi")
         package_info = client.package_releases(package_name)
         if package_info:
@@ -19,20 +20,23 @@
 def check_package_version(package_name):
     latest_version = get_latest_version(package_name)
 
     if latest_version is None:
         pass
     else:
         # 获取当前版本号。
-        current_version = pkg_resources.get_distribution(package_name).version
+
+        current_version = importlib.metadata.version(package_name)
+        # current_version = pkg_resources.get_distribution(package_name).version
         if current_version < latest_version:
             print(
                 f"'{package_name}' is outdated. latest version is {current_version} -> {latest_version}."
             )
             print(
                 f"You should consider upgrading using 'pip install --upgrade {package_name}'."
             )
 
 
 def get_current_version(package_name):
-    current_version = pkg_resources.get_distribution(package_name).version
+    # current_version = pkg_resources.get_distribution(package_name).version
+    current_version = importlib.metadata.version(package_name)
     return current_version
```

### Comparing `gentccode-0.2.6/gentccode/cli.py` & `gentccode-0.2.7/src/gentccode/cli.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.6/gentccode/convert_to_jmx.py` & `gentccode-0.2.7/src/gentccode/convert_to_jmx.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.6/gentccode/convert_to_locust.py` & `gentccode-0.2.7/src/gentccode/convert_to_locust.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.6/gentccode/generate_case_code.py` & `gentccode-0.2.7/src/gentccode/generate_case_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,13 +414,13 @@
         return new_k, new_v
 
 
 if __name__ == "__main__":
     a = GenerateCaseCode()
     # 接口信息
     api_yaml_file_path = (
-        "merged.yaml"
+        "/Users/lei.susl/vs_workspace/company/apiTest/testcase/iac/tocex_master/api.yaml"
     )
     # 生成的接口代码会保存到这个文件中
-    case_file_path = "./case_template.py"
+    case_file_path = "case_template.py"
     rule_tool = NoneRule()
     a.produce_code_for_api_yaml(api_yaml_file_path, case_file_path, rule_tool)
```

### Comparing `gentccode-0.2.6/gentccode/merge_api.py` & `gentccode-0.2.7/src/gentccode/merge_api.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.6/gentccode/produce_search_case.py` & `gentccode-0.2.7/src/gentccode/produce_search_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.6/gentccode/produce_test_case.py` & `gentccode-0.2.7/src/gentccode/produce_test_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.6/gentccode/read_swagger_rule.py` & `gentccode-0.2.7/src/gentccode/read_swagger_rule.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.6/pyproject.toml` & `gentccode-0.2.7/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [tool.poetry]
 name = "gentccode"
-version = "0.2.6"
+version = "0.2.7"
 description = "generate test case code"
 authors = ["Lei Su <lei.susl@shopee.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyyaml = "^6.0"
-http-content-parser = "^0.0.15"
+http-content-parser = "^0.0.17"
 click = "^8.1.7"
 lxml = "^4.9.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 
 [tool.poetry.scripts]
-gtc="gentccode.cli:main"
+gtc = "gentccode.cli:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+pythonpath = [".", "src"]
```

### Comparing `gentccode-0.2.6/PKG-INFO` & `gentccode-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gentccode
-Version: 0.2.6
+Version: 0.2.7
 Summary: generate test case code
 Author: Lei Su
 Author-email: lei.susl@shopee.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: http-content-parser (>=0.0.15,<0.0.16)
+Requires-Dist: http-content-parser (>=0.0.17,<0.0.18)
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 ## 简介
 
 gtc(generate test case) 是一个把http请求转换为测试代码的cli工具
```

