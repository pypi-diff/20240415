# Comparing `tmp/omitme-0.0.8.tar.gz` & `tmp/omitme-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omitme-0.0.8.tar", max compression
+gzip compressed data, was "omitme-0.0.9.tar", max compression
```

## Comparing `omitme-0.0.8.tar` & `omitme-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      610 2023-12-11 22:03:37.388274 omitme-0.0.8/LICENSE
--rw-r--r--   0        0        0     2866 2023-12-11 22:03:37.388274 omitme-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-12-11 22:03:37.388274 omitme-0.0.8/omitme/__init__.py
--rw-r--r--   0        0        0       83 2023-12-11 22:03:37.388274 omitme-0.0.8/omitme/__main__.py
--rw-r--r--   0        0        0     3982 2023-12-11 22:03:37.388274 omitme-0.0.8/omitme/cli/__init__.py
--rw-r--r--   0        0        0      270 2023-12-11 22:03:37.388274 omitme-0.0.8/omitme/errors.py
--rw-r--r--   0        0        0     9183 2023-12-11 22:03:37.388274 omitme-0.0.8/omitme/gui/app.py
--rw-r--r--   0        0        0      360 2023-12-11 22:03:37.392274 omitme-0.0.8/omitme/platforms/__init__.py
--rw-r--r--   0        0        0     5829 2023-12-11 22:03:37.392274 omitme-0.0.8/omitme/platforms/discord.py
--rw-r--r--   0        0        0      160 2023-12-11 22:03:37.392274 omitme-0.0.8/omitme/platforms/element.py
--rw-r--r--   0        0        0     2244 2023-12-11 22:03:37.392274 omitme-0.0.8/omitme/platforms/matrix.py
--rw-r--r--   0        0        0     3215 2023-12-11 22:03:37.392274 omitme-0.0.8/omitme/platforms/reddit.py
--rw-r--r--   0        0        0        0 2023-12-11 22:03:37.392274 omitme-0.0.8/omitme/platforms/twitter.py
--rw-r--r--   0        0        0        0 2023-12-11 22:03:37.392274 omitme-0.0.8/omitme/resources/__init__.py
--rw-r--r--   0        0        0   445986 2023-12-11 22:03:37.392274 omitme-0.0.8/omitme/resources/omitme.icns
--rw-r--r--   0        0        0    13871 2023-12-11 22:03:37.392274 omitme-0.0.8/omitme/resources/omitme.ico
--rw-r--r--   0        0        0    14040 2023-12-11 22:03:37.392274 omitme-0.0.8/omitme/resources/omitme.png
--rw-r--r--   0        0        0    24403 2023-12-11 22:03:37.392274 omitme-0.0.8/omitme/resources/platforms/discord.png
--rw-r--r--   0        0        0    17013 2023-12-11 22:03:37.392274 omitme-0.0.8/omitme/resources/platforms/element.png
--rw-r--r--   0        0        0     2580 2023-12-11 22:03:37.392274 omitme-0.0.8/omitme/resources/platforms/matrix.png
--rw-r--r--   0        0        0    50283 2023-12-11 22:03:37.396274 omitme-0.0.8/omitme/resources/platforms/reddit.png
--rw-r--r--   0        0        0     2013 2023-12-11 22:03:37.396274 omitme-0.0.8/omitme/util/accounts.py
--rw-r--r--   0        0        0      306 2023-12-11 22:03:37.396274 omitme-0.0.8/omitme/util/events.py
--rw-r--r--   0        0        0     1654 2023-12-11 22:03:37.396274 omitme-0.0.8/omitme/util/platform.py
--rw-r--r--   0        0        0     1975 2023-12-11 22:03:37.396274 omitme-0.0.8/omitme/util/targets.py
--rw-r--r--   0        0        0      732 2023-12-11 22:03:37.396274 omitme-0.0.8/omitme/util/wait_for.py
--rw-r--r--   0        0        0     4618 2023-12-11 22:03:37.396274 omitme-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3798 1970-01-01 00:00:00.000000 omitme-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      610 2024-04-15 08:23:20.825118 omitme-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2866 2024-04-15 08:23:20.825118 omitme-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 08:23:20.825118 omitme-0.0.9/omitme/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-15 08:23:20.825118 omitme-0.0.9/omitme/__main__.py
+-rw-r--r--   0        0        0     3982 2024-04-15 08:23:20.825118 omitme-0.0.9/omitme/cli/__init__.py
+-rw-r--r--   0        0        0      270 2024-04-15 08:23:20.825118 omitme-0.0.9/omitme/errors.py
+-rw-r--r--   0        0        0     9183 2024-04-15 08:23:20.825118 omitme-0.0.9/omitme/gui/app.py
+-rw-r--r--   0        0        0      360 2024-04-15 08:23:20.825118 omitme-0.0.9/omitme/platforms/__init__.py
+-rw-r--r--   0        0        0     5829 2024-04-15 08:23:20.825118 omitme-0.0.9/omitme/platforms/discord.py
+-rw-r--r--   0        0        0      160 2024-04-15 08:23:20.825118 omitme-0.0.9/omitme/platforms/element.py
+-rw-r--r--   0        0        0     2244 2024-04-15 08:23:20.825118 omitme-0.0.9/omitme/platforms/matrix.py
+-rw-r--r--   0        0        0     3215 2024-04-15 08:23:20.825118 omitme-0.0.9/omitme/platforms/reddit.py
+-rw-r--r--   0        0        0        0 2024-04-15 08:23:20.825118 omitme-0.0.9/omitme/platforms/twitter.py
+-rw-r--r--   0        0        0        0 2024-04-15 08:23:20.825118 omitme-0.0.9/omitme/resources/__init__.py
+-rw-r--r--   0        0        0   445986 2024-04-15 08:23:20.829118 omitme-0.0.9/omitme/resources/omitme.icns
+-rw-r--r--   0        0        0    13871 2024-04-15 08:23:20.829118 omitme-0.0.9/omitme/resources/omitme.ico
+-rw-r--r--   0        0        0    14040 2024-04-15 08:23:20.829118 omitme-0.0.9/omitme/resources/omitme.png
+-rw-r--r--   0        0        0    24403 2024-04-15 08:23:20.829118 omitme-0.0.9/omitme/resources/platforms/discord.png
+-rw-r--r--   0        0        0    17013 2024-04-15 08:23:20.829118 omitme-0.0.9/omitme/resources/platforms/element.png
+-rw-r--r--   0        0        0     2580 2024-04-15 08:23:20.829118 omitme-0.0.9/omitme/resources/platforms/matrix.png
+-rw-r--r--   0        0        0    50283 2024-04-15 08:23:20.829118 omitme-0.0.9/omitme/resources/platforms/reddit.png
+-rw-r--r--   0        0        0     2013 2024-04-15 08:23:20.829118 omitme-0.0.9/omitme/util/accounts.py
+-rw-r--r--   0        0        0      306 2024-04-15 08:23:20.829118 omitme-0.0.9/omitme/util/events.py
+-rw-r--r--   0        0        0     1654 2024-04-15 08:23:20.829118 omitme-0.0.9/omitme/util/platform.py
+-rw-r--r--   0        0        0     1975 2024-04-15 08:23:20.829118 omitme-0.0.9/omitme/util/targets.py
+-rw-r--r--   0        0        0      732 2024-04-15 08:23:20.829118 omitme-0.0.9/omitme/util/wait_for.py
+-rw-r--r--   0        0        0     4636 2024-04-15 08:23:20.829118 omitme-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 omitme-0.0.9/PKG-INFO
```

### Comparing `omitme-0.0.8/LICENSE` & `omitme-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/README.md` & `omitme-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/cli/__init__.py` & `omitme-0.0.9/omitme/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/gui/app.py` & `omitme-0.0.9/omitme/gui/app.py`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/platforms/discord.py` & `omitme-0.0.9/omitme/platforms/discord.py`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/platforms/matrix.py` & `omitme-0.0.9/omitme/platforms/matrix.py`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/platforms/reddit.py` & `omitme-0.0.9/omitme/platforms/reddit.py`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/resources/omitme.icns` & `omitme-0.0.9/omitme/resources/omitme.icns`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/resources/omitme.ico` & `omitme-0.0.9/omitme/resources/omitme.ico`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/resources/omitme.png` & `omitme-0.0.9/omitme/resources/omitme.png`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/resources/platforms/discord.png` & `omitme-0.0.9/omitme/resources/platforms/discord.png`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/resources/platforms/element.png` & `omitme-0.0.9/omitme/resources/platforms/element.png`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/resources/platforms/matrix.png` & `omitme-0.0.9/omitme/resources/platforms/matrix.png`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/resources/platforms/reddit.png` & `omitme-0.0.9/omitme/resources/platforms/reddit.png`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/util/accounts.py` & `omitme-0.0.9/omitme/util/accounts.py`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/util/platform.py` & `omitme-0.0.9/omitme/util/platform.py`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/util/targets.py` & `omitme-0.0.9/omitme/util/targets.py`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/omitme/util/wait_for.py` & `omitme-0.0.9/omitme/util/wait_for.py`

 * *Files identical despite different names*

### Comparing `omitme-0.0.8/pyproject.toml` & `omitme-0.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.briefcase]
 project_name = "Omit me"
 bundle = "com.wardpearce.omitme"
-version = "0.0.1"
+version = "0.0.9"
 url = "https://github.com/WardPearce/omitme"
 license = "GNU General Public License v3 (GPLv3)"
 author = "WardPearce"
 author_email = "wardpearce@pm.me"
 
 [tool.briefcase.app.omitme]
 formal_name = "Omit me"
@@ -152,38 +152,38 @@
 requires = [
     "toga-web~=0.3.1",
 ]
 style_framework = "Shoelace v2.3"
 
 [tool.poetry]
 name = "omitme"
-version = "0.0.8"
+version = "0.0.9"
 description = "OmitMe - Your Privacy-Centric, Easily Extendable Data Deletion Solution"
 authors = ["WardPearce <wardpearce@pm.me>"]
 license = "GNU General Public License v3 (GPLv3)"
 readme = "README.md"
 
 [tool.poetry.scripts]
 omitme-cli = "omitme:cli.main"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 selenium = "^4.11.2"
 selenium-wire = "^5.1.0"
 pydantic = "^2.1.1"
-httpx = ">=0.24.1,<0.26.0"
+httpx = ">=0.24.1,<0.28.0"
 click = "^8.1.7"
 aiofiles = "^23.2.1"
 yarl = "^1.9.2"
-keyring = {extras = ["completion"], version = "^24.2.0"}
-cryptography = "^41.0.3"
+keyring = {extras = ["completion"], version = ">=24.2,<26.0"}
+cryptography = ">=41.0.3,<43.0.0"
 setuptools = ">=68.2.2,<70.0.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.0"
+pytest = ">=7.4,<9.0"
 
 [tool.poetry.group.gui]
 optional = true
 
 [tool.poetry.group.gui.dependencies]
 toga = ">=0.3.1,<0.5.0"
 briefcase = "^0.3.15"
```

### Comparing `omitme-0.0.8/PKG-INFO` & `omitme-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: omitme
-Version: 0.0.8
+Version: 0.0.9
 Summary: OmitMe - Your Privacy-Centric, Easily Extendable Data Deletion Solution
 License: GNU General Public License v3 (GPLv3)
 Author: WardPearce
 Author-email: wardpearce@pm.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: cryptography (>=41.0.3,<42.0.0)
-Requires-Dist: httpx (>=0.24.1,<0.26.0)
-Requires-Dist: keyring[completion] (>=24.2.0,<25.0.0)
+Requires-Dist: cryptography (>=41.0.3,<43.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.28.0)
+Requires-Dist: keyring[completion] (>=24.2,<26.0)
 Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: selenium (>=4.11.2,<5.0.0)
 Requires-Dist: selenium-wire (>=5.1.0,<6.0.0)
 Requires-Dist: setuptools (>=68.2.2,<70.0.0)
 Requires-Dist: yarl (>=1.9.2,<2.0.0)
 Description-Content-Type: text/markdown
```

