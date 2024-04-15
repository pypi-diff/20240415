# Comparing `tmp/cz_kpn-3.2.4.tar.gz` & `tmp/cz_kpn-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz_kpn-3.2.4.tar", max compression
+gzip compressed data, was "cz_kpn-3.2.5.tar", max compression
```

## Comparing `cz_kpn-3.2.4.tar` & `cz_kpn-3.2.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1272 2024-01-03 13:50:13.969849 cz_kpn-3.2.4/CHANGELOG.md
--rw-r--r--   0        0        0     1059 2024-01-03 13:50:13.973849 cz_kpn-3.2.4/LICENSE
--rw-r--r--   0        0        0     6272 2024-01-03 13:50:13.973849 cz_kpn-3.2.4/README.md
--rw-r--r--   0        0        0   564052 2024-01-03 13:50:13.973849 cz_kpn-3.2.4/docs/images/bump.gif
--rw-r--r--   0        0        0  1023699 2024-01-03 13:50:13.977849 cz_kpn-3.2.4/docs/images/commit.gif
--rw-r--r--   0        0        0      920 2024-01-03 13:50:13.977849 cz_kpn-3.2.4/pyproject.toml
--rw-r--r--   0        0        0       52 2024-01-03 13:50:13.977849 cz_kpn-3.2.4/src/cz_kpn/__init__.py
--rw-r--r--   0        0        0      763 2024-01-03 13:50:13.977849 cz_kpn-3.2.4/src/cz_kpn/consts.py
--rw-r--r--   0        0        0     1359 2024-01-03 13:50:13.977849 cz_kpn-3.2.4/src/cz_kpn/cz_kpn_info.txt
--rw-r--r--   0        0        0     3423 2024-01-03 13:50:13.977849 cz_kpn-3.2.4/src/cz_kpn/rules.py
--rw-r--r--   0        0        0     7182 1970-01-01 00:00:00.000000 cz_kpn-3.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1417 2024-04-15 09:22:53.250926 cz_kpn-3.2.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1059 2024-04-15 09:22:53.250926 cz_kpn-3.2.5/LICENSE
+-rw-r--r--   0        0        0     6272 2024-04-15 09:22:53.250926 cz_kpn-3.2.5/README.md
+-rw-r--r--   0        0        0   564052 2024-04-15 09:22:53.250926 cz_kpn-3.2.5/docs/images/bump.gif
+-rw-r--r--   0        0        0  1023699 2024-04-15 09:22:53.254926 cz_kpn-3.2.5/docs/images/commit.gif
+-rw-r--r--   0        0        0      920 2024-04-15 09:22:53.254926 cz_kpn-3.2.5/pyproject.toml
+-rw-r--r--   0        0        0       52 2024-04-15 09:22:53.254926 cz_kpn-3.2.5/src/cz_kpn/__init__.py
+-rw-r--r--   0        0        0      763 2024-04-15 09:22:53.254926 cz_kpn-3.2.5/src/cz_kpn/consts.py
+-rw-r--r--   0        0        0     1359 2024-04-15 09:22:53.254926 cz_kpn-3.2.5/src/cz_kpn/cz_kpn_info.txt
+-rw-r--r--   0        0        0     3423 2024-04-15 09:22:53.254926 cz_kpn-3.2.5/src/cz_kpn/rules.py
+-rw-r--r--   0        0        0     7182 1970-01-01 00:00:00.000000 cz_kpn-3.2.5/PKG-INFO
```

### Comparing `cz_kpn-3.2.4/CHANGELOG.md` & `cz_kpn-3.2.5/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 3.2.5 (2024-04-15)
+
+### Fixes
+
+- release pipeline ([1ab09a8](https://github.com/kpn/cz-kpn/commit/1ab09a840ba1e83ed57f524b5dba7fd385940ab0))
+
 ## 3.2.4 (2024-01-03)
 
 ### Improvements
 
 - Bump docker github action ([4474f52](https://github.com/kpn/cz-kpn/commit/4474f52cf3334aaa5713651b3642d5ff1cf75256))
 
 ## 3.2.3 (2023-09-08)
```

### Comparing `cz_kpn-3.2.4/LICENSE` & `cz_kpn-3.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.4/README.md` & `cz_kpn-3.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.4/docs/images/bump.gif` & `cz_kpn-3.2.5/docs/images/bump.gif`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.4/docs/images/commit.gif` & `cz_kpn-3.2.5/docs/images/commit.gif`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.4/pyproject.toml` & `cz_kpn-3.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cz-kpn"
-version = "3.2.4"
+version = "3.2.5"
 description = "commitizen with kpn style"
 authors = ["Santiago Fraire Willemoes <santiago.fraire@kpn.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "cz_kpn", from = "src" }]
 classifiers = [
     "Topic :: Software Development :: Build Tools",
```

### Comparing `cz_kpn-3.2.4/src/cz_kpn/consts.py` & `cz_kpn-3.2.5/src/cz_kpn/consts.py`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.4/src/cz_kpn/cz_kpn_info.txt` & `cz_kpn-3.2.5/src/cz_kpn/cz_kpn_info.txt`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.4/src/cz_kpn/rules.py` & `cz_kpn-3.2.5/src/cz_kpn/rules.py`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.4/PKG-INFO` & `cz_kpn-3.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cz-kpn
-Version: 3.2.4
+Version: 3.2.5
 Summary: commitizen with kpn style
 Home-page: https://github.com/kpn/cz-kpn
 License: MIT
 Keywords: commitizen,release-management,autorelease
 Author: Santiago Fraire Willemoes
 Author-email: santiago.fraire@kpn.com
 Requires-Python: >=3.9,<4.0
```

