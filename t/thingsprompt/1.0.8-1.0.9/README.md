# Comparing `tmp/thingsprompt-1.0.8.tar.gz` & `tmp/thingsprompt-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingsprompt-1.0.8.tar", last modified: Thu Feb 29 14:04:26 2024, max compression
+gzip compressed data, was "thingsprompt-1.0.9.tar", last modified: Thu Feb 29 14:31:10 2024, max compression
```

## Comparing `thingsprompt-1.0.8.tar` & `thingsprompt-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-02-29 14:04:26.543641 thingsprompt-1.0.8/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-02-29 14:04:26.543641 thingsprompt-1.0.8/.github/
--rw-rw-r--   0 joente    (1000) joente    (1000)       15 2022-10-07 08:06:09.000000 thingsprompt-1.0.8/.github/FUNDING.yml
--rw-rw-r--   0 joente    (1000) joente    (1000)     1203 2019-07-16 19:49:06.000000 thingsprompt-1.0.8/.gitignore
--rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2020-01-31 09:24:30.000000 thingsprompt-1.0.8/LICENSE
--rw-r--r--   0 joente    (1000) joente    (1000)     4679 2024-02-29 14:04:26.543641 thingsprompt-1.0.8/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)     3811 2024-02-23 10:12:34.000000 thingsprompt-1.0.8/README.md
--rw-rw-r--   0 joente    (1000) joente    (1000)       76 2024-01-09 14:29:27.000000 thingsprompt-1.0.8/requirements.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       38 2024-02-29 14:04:26.543641 thingsprompt-1.0.8/setup.cfg
--rw-rw-r--   0 joente    (1000) joente    (1000)     1864 2024-02-29 14:01:13.000000 thingsprompt-1.0.8/setup.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-02-29 14:04:26.543641 thingsprompt-1.0.8/thingsprompt/
--rwxrwxr-x   0 joente    (1000) joente    (1000)    18142 2024-02-29 14:01:10.000000 thingsprompt-1.0.8/thingsprompt/__init__.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-02-29 14:04:26.543641 thingsprompt-1.0.8/thingsprompt.egg-info/
--rw-r--r--   0 joente    (1000) joente    (1000)     4679 2024-02-29 14:04:26.000000 thingsprompt-1.0.8/thingsprompt.egg-info/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)      317 2024-02-29 14:04:26.000000 thingsprompt-1.0.8/thingsprompt.egg-info/SOURCES.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        1 2024-02-29 14:04:26.000000 thingsprompt-1.0.8/thingsprompt.egg-info/dependency_links.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       52 2024-02-29 14:04:26.000000 thingsprompt-1.0.8/thingsprompt.egg-info/entry_points.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       53 2024-02-29 14:04:26.000000 thingsprompt-1.0.8/thingsprompt.egg-info/requires.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       13 2024-02-29 14:04:26.000000 thingsprompt-1.0.8/thingsprompt.egg-info/top_level.txt
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-02-29 14:31:10.531414 thingsprompt-1.0.9/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-02-29 14:31:10.531414 thingsprompt-1.0.9/.github/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       15 2022-10-07 08:06:09.000000 thingsprompt-1.0.9/.github/FUNDING.yml
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1203 2019-07-16 19:49:06.000000 thingsprompt-1.0.9/.gitignore
+-rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2020-01-31 09:24:30.000000 thingsprompt-1.0.9/LICENSE
+-rw-r--r--   0 joente    (1000) joente    (1000)     4679 2024-02-29 14:31:10.531414 thingsprompt-1.0.9/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3811 2024-02-23 10:12:34.000000 thingsprompt-1.0.9/README.md
+-rw-rw-r--   0 joente    (1000) joente    (1000)       76 2024-01-09 14:29:27.000000 thingsprompt-1.0.9/requirements.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       38 2024-02-29 14:31:10.531414 thingsprompt-1.0.9/setup.cfg
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1922 2024-02-29 14:31:04.000000 thingsprompt-1.0.9/setup.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-02-29 14:31:10.531414 thingsprompt-1.0.9/thingsprompt/
+-rw-rw-r--   0 joente    (1000) joente    (1000)        0 2024-02-29 14:25:29.000000 thingsprompt-1.0.9/thingsprompt/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       70 2024-02-29 14:29:13.000000 thingsprompt-1.0.9/thingsprompt/__main__.py
+-rwxrwxr-x   0 joente    (1000) joente    (1000)    18142 2024-02-29 14:26:40.000000 thingsprompt-1.0.9/thingsprompt/thingsprompt.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-02-29 14:31:10.531414 thingsprompt-1.0.9/thingsprompt.egg-info/
+-rw-r--r--   0 joente    (1000) joente    (1000)     4679 2024-02-29 14:31:10.000000 thingsprompt-1.0.9/thingsprompt.egg-info/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)      371 2024-02-29 14:31:10.000000 thingsprompt-1.0.9/thingsprompt.egg-info/SOURCES.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        1 2024-02-29 14:31:10.000000 thingsprompt-1.0.9/thingsprompt.egg-info/dependency_links.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       65 2024-02-29 14:31:10.000000 thingsprompt-1.0.9/thingsprompt.egg-info/entry_points.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       53 2024-02-29 14:31:10.000000 thingsprompt-1.0.9/thingsprompt.egg-info/requires.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       13 2024-02-29 14:31:10.000000 thingsprompt-1.0.9/thingsprompt.egg-info/top_level.txt
```

### Comparing `thingsprompt-1.0.8/.gitignore` & `thingsprompt-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `thingsprompt-1.0.8/LICENSE` & `thingsprompt-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `thingsprompt-1.0.8/PKG-INFO` & `thingsprompt-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsprompt
-Version: 1.0.8
+Version: 1.0.9
 Summary: ThingsDB Prompt
 Home-page: https://github.com/thingsdb/ThingsPrompt
 Author: Jeroen van der Heijden
 Author-email: jeroen@cesbit.com
 License: GPLv3
 Keywords: database connector prompt thingsdb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `thingsprompt-1.0.8/README.md` & `thingsprompt-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `thingsprompt-1.0.8/setup.py` & `thingsprompt-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 Upload to PyPI
 
 pip -v install --use-pep517 -e .
 python setup.py sdist
 twine upload --repository pypitest dist/thingsprompt-X.X.X.tar.gz
 twine upload --repository pypi dist/thingsprompt-X.X.X.tar.gz
 """
-from setuptools import setup
+from setuptools import setup, find_packages
 
 try:
     with open('README.md', 'r') as f:
         long_description = f.read()
 except IOError:
     long_description = ''
 
 setup(
     name='thingsprompt',
-    version='1.0.8',  # Update version in thingsprompt as well
+    version='1.0.9',  # Update version in thingsprompt as well
     description='ThingsDB Prompt',
     url='https://github.com/thingsdb/ThingsPrompt',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jeroen van der Heijden',
     author_email='jeroen@cesbit.com',
     entry_points = {
-        'console_scripts': ['things-prompt=thingsprompt:main'],
+        'console_scripts': ['things-prompt=thingsprompt.thingsprompt:main'],
     },
     license='GPLv3',
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
@@ -45,14 +45,15 @@
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
+    packages=find_packages(),
     install_requires=[
         'setproctitle',
         'python-thingsdb',
         'prompt-toolkit',
         'pygments',
     ],
     keywords='database connector prompt thingsdb',
```

### Comparing `thingsprompt-1.0.8/thingsprompt/__init__.py` & `thingsprompt-1.0.9/thingsprompt/thingsprompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from prompt_toolkit.styles.pygments import style_from_pygments_cls
 from pygments.styles import get_style_by_name
 from pygments.lexer import RegexLexer, include, bygroups
 from pygments.token import Comment, Keyword, Name, Number, String, Text, \
     Operator, Punctuation, Whitespace
 
 
-__version__ = '1.0.8'  # keep equal to the one in setup.py
+__version__ = '1.0.9'  # keep equal to the one in setup.py
 
 
 class ThingsDBLexer(RegexLexer):
     """
     Lexer for the ThingsDB programming language.
 
     .. versionadded:: 2.9
```

### Comparing `thingsprompt-1.0.8/thingsprompt.egg-info/PKG-INFO` & `thingsprompt-1.0.9/thingsprompt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsprompt
-Version: 1.0.8
+Version: 1.0.9
 Summary: ThingsDB Prompt
 Home-page: https://github.com/thingsdb/ThingsPrompt
 Author: Jeroen van der Heijden
 Author-email: jeroen@cesbit.com
 License: GPLv3
 Keywords: database connector prompt thingsdb
 Classifier: Development Status :: 4 - Beta
```

