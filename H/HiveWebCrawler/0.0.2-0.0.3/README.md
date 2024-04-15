# Comparing `tmp/hivewebcrawler-0.0.2.tar.gz` & `tmp/hivewebcrawler-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivewebcrawler-0.0.2.tar", last modified: Mon Apr 15 10:52:21 2024, max compression
+gzip compressed data, was "hivewebcrawler-0.0.3.tar", last modified: Mon Apr 15 13:17:28 2024, max compression
```

## Comparing `hivewebcrawler-0.0.2.tar` & `hivewebcrawler-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 10:52:21.774059 hivewebcrawler-0.0.2/
-drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 10:52:21.774059 hivewebcrawler-0.0.2/HiveWebCrawler/
-drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 10:52:21.774059 hivewebcrawler-0.0.2/HiveWebCrawler/HiveWebCrawler.egg-info/
--rw-r--r--   0 delta     (1000) delta     (1000)      685 2024-04-15 10:52:21.000000 hivewebcrawler-0.0.2/HiveWebCrawler/HiveWebCrawler.egg-info/PKG-INFO
--rw-r--r--   0 delta     (1000) delta     (1000)      282 2024-04-15 10:52:21.000000 hivewebcrawler-0.0.2/HiveWebCrawler/HiveWebCrawler.egg-info/SOURCES.txt
--rw-r--r--   0 delta     (1000) delta     (1000)        1 2024-04-15 10:52:21.000000 hivewebcrawler-0.0.2/HiveWebCrawler/HiveWebCrawler.egg-info/dependency_links.txt
--rw-r--r--   0 delta     (1000) delta     (1000)       24 2024-04-15 10:52:21.000000 hivewebcrawler-0.0.2/HiveWebCrawler/HiveWebCrawler.egg-info/requires.txt
--rw-r--r--   0 delta     (1000) delta     (1000)        1 2024-04-15 10:52:21.000000 hivewebcrawler-0.0.2/HiveWebCrawler/HiveWebCrawler.egg-info/top_level.txt
--rw-r--r--   0 delta     (1000) delta     (1000)      685 2024-04-15 10:52:21.774059 hivewebcrawler-0.0.2/PKG-INFO
--rw-r--r--   0 delta     (1000) delta     (1000)       58 2024-04-15 10:03:56.000000 hivewebcrawler-0.0.2/README.md
--rw-r--r--   0 delta     (1000) delta     (1000)       38 2024-04-15 10:52:21.774059 hivewebcrawler-0.0.2/setup.cfg
--rw-r--r--   0 delta     (1000) delta     (1000)     1048 2024-04-15 10:52:12.000000 hivewebcrawler-0.0.2/setup.py
+drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 13:17:28.395203 hivewebcrawler-0.0.3/
+drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 13:17:28.395203 hivewebcrawler-0.0.3/HiveWebCrawler/
+-rw-r--r--   0 delta     (1000) delta     (1000)    12384 2024-04-15 09:46:49.000000 hivewebcrawler-0.0.3/HiveWebCrawler/Crawler.py
+-rw-r--r--   0 delta     (1000) delta     (1000)       24 2024-04-15 12:55:31.000000 hivewebcrawler-0.0.3/HiveWebCrawler/__init__.py
+drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 13:17:28.395203 hivewebcrawler-0.0.3/HiveWebCrawler.egg-info/
+-rw-r--r--   0 delta     (1000) delta     (1000)     5851 2024-04-15 13:17:28.000000 hivewebcrawler-0.0.3/HiveWebCrawler.egg-info/PKG-INFO
+-rw-r--r--   0 delta     (1000) delta     (1000)      273 2024-04-15 13:17:28.000000 hivewebcrawler-0.0.3/HiveWebCrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 delta     (1000) delta     (1000)        1 2024-04-15 13:17:28.000000 hivewebcrawler-0.0.3/HiveWebCrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 delta     (1000) delta     (1000)       24 2024-04-15 13:17:28.000000 hivewebcrawler-0.0.3/HiveWebCrawler.egg-info/requires.txt
+-rw-r--r--   0 delta     (1000) delta     (1000)       15 2024-04-15 13:17:28.000000 hivewebcrawler-0.0.3/HiveWebCrawler.egg-info/top_level.txt
+-rw-r--r--   0 delta     (1000) delta     (1000)     5851 2024-04-15 13:17:28.395203 hivewebcrawler-0.0.3/PKG-INFO
+-rw-r--r--   0 delta     (1000) delta     (1000)     5190 2024-04-15 13:16:27.000000 hivewebcrawler-0.0.3/README.md
+-rw-r--r--   0 delta     (1000) delta     (1000)       38 2024-04-15 13:17:28.395203 hivewebcrawler-0.0.3/setup.cfg
+-rw-r--r--   0 delta     (1000) delta     (1000)      981 2024-04-15 13:16:54.000000 hivewebcrawler-0.0.3/setup.py
+drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 13:17:28.395203 hivewebcrawler-0.0.3/test/
+-rw-r--r--   0 delta     (1000) delta     (1000)      559 2024-04-15 13:15:46.000000 hivewebcrawler-0.0.3/test/test.py
```

### Comparing `hivewebcrawler-0.0.2/setup.py` & `hivewebcrawler-0.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import setuptools
 
-long_describe = ""
-long_describe_format = "text/markdown"
+long_describe = ''
+long_describe_format = 'text/markdown'
 
-with open("README.md","r") as readmeFile:
+with open('README.md','r') as readmeFile:
     long_describe = readmeFile.read()
 
 setuptools.setup(
-    name="HiveWebCrawler",
-    author="MehmetYukselSekeroglu",
-    version="0.0.2",
-    author_email="dijital_evren@protonmail.com",
-    description="Simple Python 3.x Web Crawler, Images, Urls, Emails, Phone numbers",
+    name='HiveWebCrawler',
+    author='MehmetYukselSekeroglu',
+    version='0.0.3',
+    author_email='dijital_evren@protonmail.com',
+    description='Python 3.x Web Crawler, Images, Urls, Emails, Phone numbers',
     long_description=long_describe,
-    long_descriptlion_content_type=long_describe_format,
-    keywords="PyPi, Web Crawler, Web Image Crawler, Web URL Crawler, Web Email Crawler, Web Phone Number Crawler",
+    long_description_content_type=long_describe_format,
+    keywords='PyPi, Web Crawler, Web Image Crawler, Web URL Crawler, Web Email Crawler, Web Phone Number Crawler',
     project_urls={
-        "Bug Reports":"https://github.com/MehmetYukselSekeroglu/HiveWebCrawler/issues",
-        "Source Code":"https://github.com/MehmetYukselSekeroglu/HiveWebCrawler"
+        'Bug Reports':'https://github.com/MehmetYukselSekeroglu/HiveWebCrawler/issues',
+        'Source Code':'https://github.com/MehmetYukselSekeroglu/HiveWebCrawler'
     },
-    url="https://github.com/MehmetYukselSekeroglu/HiveWebCrawler",
-    package_dir={"":"HiveWebCrawler"},
-    packages=setuptools.find_packages(where="HiveWebCrawler"),
-    python_requires=">=3.8",
-    install_requires=["requests","beautifulsoup4"]
+    url='https://github.com/MehmetYukselSekeroglu/HiveWebCrawler',
+    packages=setuptools.find_packages(),
+    python_requires='>=3.8',
+    install_requires=['requests','beautifulsoup4'], 
 )
```

