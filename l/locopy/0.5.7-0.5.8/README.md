# Comparing `tmp/locopy-0.5.7.tar.gz` & `tmp/locopy-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locopy-0.5.7.tar", last modified: Tue Jan 23 14:56:00 2024, max compression
+gzip compressed data, was "locopy-0.5.8.tar", last modified: Mon Apr 15 14:55:38 2024, max compression
```

## Comparing `locopy-0.5.7.tar` & `locopy-0.5.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 14:56:00.411523 locopy-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-23 14:55:29.000000 locopy-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-23 14:55:29.000000 locopy-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-01-23 14:56:00.411523 locopy-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-01-23 14:55:29.000000 locopy-0.5.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 14:56:00.403524 locopy-0.5.7/locopy/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-23 14:55:29.000000 locopy-0.5.7/locopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-01-23 14:55:29.000000 locopy-0.5.7/locopy/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-01-23 14:55:29.000000 locopy-0.5.7/locopy/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-01-23 14:55:29.000000 locopy-0.5.7/locopy/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-01-23 14:55:29.000000 locopy-0.5.7/locopy/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    21755 2024-01-23 14:55:29.000000 locopy-0.5.7/locopy/redshift.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-01-23 14:55:29.000000 locopy-0.5.7/locopy/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-01-23 14:55:29.000000 locopy-0.5.7/locopy/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-01-23 14:55:29.000000 locopy-0.5.7/locopy/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 14:56:00.407523 locopy-0.5.7/locopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-01-23 14:56:00.000000 locopy-0.5.7/locopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-01-23 14:56:00.000000 locopy-0.5.7/locopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 14:56:00.000000 locopy-0.5.7/locopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 14:55:34.000000 locopy-0.5.7/locopy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-23 14:56:00.000000 locopy-0.5.7/locopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-23 14:56:00.000000 locopy-0.5.7/locopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-01-23 14:55:29.000000 locopy-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-01-23 14:55:29.000000 locopy-0.5.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 14:56:00.411523 locopy-0.5.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 14:56:00.407523 locopy-0.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10347 2024-01-23 14:55:29.000000 locopy-0.5.7/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-01-23 14:55:29.000000 locopy-0.5.7/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-01-23 14:55:29.000000 locopy-0.5.7/tests/test_integration_sf.py
--rw-r--r--   0 runner    (1001) docker     (127)    36170 2024-01-23 14:55:29.000000 locopy-0.5.7/tests/test_redshift.py
--rw-r--r--   0 runner    (1001) docker     (127)    15698 2024-01-23 14:55:29.000000 locopy-0.5.7/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    18129 2024-01-23 14:55:29.000000 locopy-0.5.7/tests/test_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-01-23 14:55:29.000000 locopy-0.5.7/tests/test_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:55:38.509951 locopy-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 14:55:08.000000 locopy-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 14:55:08.000000 locopy-0.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-15 14:55:38.509951 locopy-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-15 14:55:08.000000 locopy-0.5.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:55:38.505951 locopy-0.5.8/locopy/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-15 14:55:08.000000 locopy-0.5.8/locopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-15 14:55:08.000000 locopy-0.5.8/locopy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-15 14:55:08.000000 locopy-0.5.8/locopy/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-15 14:55:08.000000 locopy-0.5.8/locopy/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-15 14:55:08.000000 locopy-0.5.8/locopy/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21755 2024-04-15 14:55:08.000000 locopy-0.5.8/locopy/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-04-15 14:55:08.000000 locopy-0.5.8/locopy/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-04-15 14:55:08.000000 locopy-0.5.8/locopy/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-04-15 14:55:08.000000 locopy-0.5.8/locopy/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:55:38.505951 locopy-0.5.8/locopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-15 14:55:38.000000 locopy-0.5.8/locopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-15 14:55:38.000000 locopy-0.5.8/locopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:55:38.000000 locopy-0.5.8/locopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:55:11.000000 locopy-0.5.8/locopy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-15 14:55:38.000000 locopy-0.5.8/locopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 14:55:38.000000 locopy-0.5.8/locopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-15 14:55:08.000000 locopy-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-15 14:55:08.000000 locopy-0.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:55:38.509951 locopy-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:55:38.505951 locopy-0.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10347 2024-04-15 14:55:08.000000 locopy-0.5.8/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-04-15 14:55:08.000000 locopy-0.5.8/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-15 14:55:08.000000 locopy-0.5.8/tests/test_integration_sf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36170 2024-04-15 14:55:08.000000 locopy-0.5.8/tests/test_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15698 2024-04-15 14:55:08.000000 locopy-0.5.8/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18129 2024-04-15 14:55:08.000000 locopy-0.5.8/tests/test_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-04-15 14:55:08.000000 locopy-0.5.8/tests/test_utility.py
```

### Comparing `locopy-0.5.7/LICENSE` & `locopy-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/PKG-INFO` & `locopy-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locopy
-Version: 0.5.7
+Version: 0.5.8
 Summary: Loading/Unloading to Amazon Redshift using Python
 Author-email: Faisal Dosani <faisal.dosani@capitalone.com>
 License: Apache Software License
 Project-URL: Homepage, https://github.com/capitalone/locopy
 Project-URL: Documentation, https://capitalone.github.io/locopy/
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -15,18 +15,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: boto3<=1.34.22,>=1.9.92
+Requires-Dist: boto3<=1.34.83,>=1.9.92
 Requires-Dist: PyYAML<=6.0.1,>=5.1
-Requires-Dist: pandas<=2.1.4,>=0.25.2
-Requires-Dist: numpy<=1.26.3,>=1.22.0
+Requires-Dist: pandas<=2.2.2,>=0.25.2
+Requires-Dist: numpy<=1.26.4,>=1.22.0
 Provides-Extra: psycopg2
 Requires-Dist: psycopg2-binary>=2.7.7; extra == "psycopg2"
 Provides-Extra: pg8000
 Requires-Dist: pg8000>=1.13.1; extra == "pg8000"
 Provides-Extra: snowflake
 Requires-Dist: snowflake-connector-python[pandas]>=2.1.2; extra == "snowflake"
 Provides-Extra: docs
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: locopy Version: 0.5.7 Summary: Loading/Unloading to
+Metadata-Version: 2.1 Name: locopy Version: 0.5.8 Summary: Loading/Unloading to
 Amazon Redshift using Python Author-email: Faisal Dosani
 capitalone.com> License: Apache Software License Project-URL: Homepage, https:/
 /github.com/capitalone/locopy Project-URL: Documentation, https://
 capitalone.github.io/locopy/ Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst License-File: LICENSE Requires-Dist:
-boto3<=1.34.22,>=1.9.92 Requires-Dist: PyYAML<=6.0.1,>=5.1 Requires-Dist:
-pandas<=2.1.4,>=0.25.2 Requires-Dist: numpy<=1.26.3,>=1.22.0 Provides-Extra:
+boto3<=1.34.83,>=1.9.92 Requires-Dist: PyYAML<=6.0.1,>=5.1 Requires-Dist:
+pandas<=2.2.2,>=0.25.2 Requires-Dist: numpy<=1.26.4,>=1.22.0 Provides-Extra:
 psycopg2 Requires-Dist: psycopg2-binary>=2.7.7; extra == "psycopg2" Provides-
 Extra: pg8000 Requires-Dist: pg8000>=1.13.1; extra == "pg8000" Provides-Extra:
 snowflake Requires-Dist: snowflake-connector-python[pandas]>=2.1.2; extra ==
 "snowflake" Provides-Extra: docs Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs" Provides-Extra: tests
 Requires-Dist: hypothesis; extra == "tests" Requires-Dist: pytest; extra ==
 "tests" Requires-Dist: pytest-cov; extra == "tests" Provides-Extra: qa
```

### Comparing `locopy-0.5.7/README.rst` & `locopy-0.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/locopy/__init__.py` & `locopy-0.5.8/locopy/__init__.py`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/locopy/_version.py` & `locopy-0.5.8/locopy/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.5.7"
+__version__ = "0.5.8"
```

### Comparing `locopy-0.5.7/locopy/database.py` & `locopy-0.5.8/locopy/database.py`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/locopy/errors.py` & `locopy-0.5.8/locopy/errors.py`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/locopy/logger.py` & `locopy-0.5.8/locopy/logger.py`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/locopy/redshift.py` & `locopy-0.5.8/locopy/redshift.py`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/locopy/s3.py` & `locopy-0.5.8/locopy/s3.py`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/locopy/snowflake.py` & `locopy-0.5.8/locopy/snowflake.py`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/locopy/utility.py` & `locopy-0.5.8/locopy/utility.py`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/locopy.egg-info/PKG-INFO` & `locopy-0.5.8/locopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locopy
-Version: 0.5.7
+Version: 0.5.8
 Summary: Loading/Unloading to Amazon Redshift using Python
 Author-email: Faisal Dosani <faisal.dosani@capitalone.com>
 License: Apache Software License
 Project-URL: Homepage, https://github.com/capitalone/locopy
 Project-URL: Documentation, https://capitalone.github.io/locopy/
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -15,18 +15,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: boto3<=1.34.22,>=1.9.92
+Requires-Dist: boto3<=1.34.83,>=1.9.92
 Requires-Dist: PyYAML<=6.0.1,>=5.1
-Requires-Dist: pandas<=2.1.4,>=0.25.2
-Requires-Dist: numpy<=1.26.3,>=1.22.0
+Requires-Dist: pandas<=2.2.2,>=0.25.2
+Requires-Dist: numpy<=1.26.4,>=1.22.0
 Provides-Extra: psycopg2
 Requires-Dist: psycopg2-binary>=2.7.7; extra == "psycopg2"
 Provides-Extra: pg8000
 Requires-Dist: pg8000>=1.13.1; extra == "pg8000"
 Provides-Extra: snowflake
 Requires-Dist: snowflake-connector-python[pandas]>=2.1.2; extra == "snowflake"
 Provides-Extra: docs
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: locopy Version: 0.5.7 Summary: Loading/Unloading to
+Metadata-Version: 2.1 Name: locopy Version: 0.5.8 Summary: Loading/Unloading to
 Amazon Redshift using Python Author-email: Faisal Dosani
 capitalone.com> License: Apache Software License Project-URL: Homepage, https:/
 /github.com/capitalone/locopy Project-URL: Documentation, https://
 capitalone.github.io/locopy/ Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst License-File: LICENSE Requires-Dist:
-boto3<=1.34.22,>=1.9.92 Requires-Dist: PyYAML<=6.0.1,>=5.1 Requires-Dist:
-pandas<=2.1.4,>=0.25.2 Requires-Dist: numpy<=1.26.3,>=1.22.0 Provides-Extra:
+boto3<=1.34.83,>=1.9.92 Requires-Dist: PyYAML<=6.0.1,>=5.1 Requires-Dist:
+pandas<=2.2.2,>=0.25.2 Requires-Dist: numpy<=1.26.4,>=1.22.0 Provides-Extra:
 psycopg2 Requires-Dist: psycopg2-binary>=2.7.7; extra == "psycopg2" Provides-
 Extra: pg8000 Requires-Dist: pg8000>=1.13.1; extra == "pg8000" Provides-Extra:
 snowflake Requires-Dist: snowflake-connector-python[pandas]>=2.1.2; extra ==
 "snowflake" Provides-Extra: docs Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs" Provides-Extra: tests
 Requires-Dist: hypothesis; extra == "tests" Requires-Dist: pytest; extra ==
 "tests" Requires-Dist: pytest-cov; extra == "tests" Provides-Extra: qa
```

### Comparing `locopy-0.5.7/locopy.egg-info/SOURCES.txt` & `locopy-0.5.8/locopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/pyproject.toml` & `locopy-0.5.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "locopy"
 description = "Loading/Unloading to Amazon Redshift using Python"
 readme = "README.rst"
 authors = [
   { name="Faisal Dosani", email="faisal.dosani@capitalone.com" },
 ]
 license = {text = "Apache Software License"}
-dependencies = ["boto3<=1.34.22,>=1.9.92", "PyYAML<=6.0.1,>=5.1", "pandas<=2.1.4,>=0.25.2", "numpy<=1.26.3,>=1.22.0"]
+dependencies = ["boto3<=1.34.83,>=1.9.92", "PyYAML<=6.0.1,>=5.1", "pandas<=2.2.2,>=0.25.2", "numpy<=1.26.4,>=1.22.0"]
 
 requires-python = ">=3.8.0"
 classifiers = [
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
```

### Comparing `locopy-0.5.7/requirements.txt` & `locopy-0.5.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/tests/test_database.py` & `locopy-0.5.8/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/tests/test_integration.py` & `locopy-0.5.8/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/tests/test_integration_sf.py` & `locopy-0.5.8/tests/test_integration_sf.py`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/tests/test_redshift.py` & `locopy-0.5.8/tests/test_redshift.py`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/tests/test_s3.py` & `locopy-0.5.8/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/tests/test_snowflake.py` & `locopy-0.5.8/tests/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `locopy-0.5.7/tests/test_utility.py` & `locopy-0.5.8/tests/test_utility.py`

 * *Files identical despite different names*

