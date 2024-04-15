# Comparing `tmp/soupsavvy-0.1.3.tar.gz` & `tmp/soupsavvy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soupsavvy-0.1.3.tar", last modified: Sun Feb 25 23:57:16 2024, max compression
+gzip compressed data, was "soupsavvy-0.1.4.tar", last modified: Mon Apr 15 15:46:49 2024, max compression
```

## Comparing `soupsavvy-0.1.3.tar` & `soupsavvy-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 23:57:16.210571 soupsavvy-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-25 23:56:59.000000 soupsavvy-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-02-25 23:57:16.210571 soupsavvy-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-02-25 23:56:59.000000 soupsavvy-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 23:57:16.206571 soupsavvy-0.1.3/config/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-25 23:56:59.000000 soupsavvy-0.1.3/config/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-25 23:56:59.000000 soupsavvy-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-25 23:56:59.000000 soupsavvy-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 23:57:16.210571 soupsavvy-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 23:57:16.206571 soupsavvy-0.1.3/soupsavvy/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-25 23:57:05.000000 soupsavvy-0.1.3/soupsavvy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 23:57:16.210571 soupsavvy-0.1.3/soupsavvy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-02-25 23:57:16.000000 soupsavvy-0.1.3/soupsavvy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-25 23:57:16.000000 soupsavvy-0.1.3/soupsavvy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 23:57:16.000000 soupsavvy-0.1.3/soupsavvy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-25 23:57:16.000000 soupsavvy-0.1.3/soupsavvy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-25 23:57:16.000000 soupsavvy-0.1.3/soupsavvy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.791740 soupsavvy-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-04-15 15:46:49.791740 soupsavvy-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:46:49.791740 soupsavvy-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.787739 soupsavvy-0.1.4/soupsavvy/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 15:46:36.000000 soupsavvy-0.1.4/soupsavvy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-15 15:46:36.000000 soupsavvy-0.1.4/soupsavvy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.787739 soupsavvy-0.1.4/soupsavvy/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/tags/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/tags/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/tags/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/tags/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.787739 soupsavvy-0.1.4/soupsavvy/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.787739 soupsavvy-0.1.4/soupsavvy/testing/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.791740 soupsavvy-0.1.4/soupsavvy/testing/generators/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/templates/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/templates/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/templates/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.791740 soupsavvy-0.1.4/soupsavvy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.791740 soupsavvy-0.1.4/soupsavvy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-04-15 15:46:49.000000 soupsavvy-0.1.4/soupsavvy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-15 15:46:49.000000 soupsavvy-0.1.4/soupsavvy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:46:49.000000 soupsavvy-0.1.4/soupsavvy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 15:46:49.000000 soupsavvy-0.1.4/soupsavvy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 15:46:49.000000 soupsavvy-0.1.4/soupsavvy.egg-info/top_level.txt
```

### Comparing `soupsavvy-0.1.3/LICENSE` & `soupsavvy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.3/PKG-INFO` & `soupsavvy-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soupsavvy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python package for advanced web scraping
 Author: sewcio543
 License: MIT License
         
         Copyright (c) 2024 Wojciech Seweryn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,32 +37,36 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.2
 Requires-Dist: lxml==4.9.2
 Provides-Extra: dev
-Requires-Dist: black==24.1.1; extra == "dev"
+Requires-Dist: black==24.3.0; extra == "dev"
 Requires-Dist: build==1.0.3; extra == "dev"
 Requires-Dist: bump2version==1.0.1; extra == "dev"
 Requires-Dist: codecov==2.1.13; extra == "dev"
 Requires-Dist: coverage==7.2.2; extra == "dev"
 Requires-Dist: flake8==7.0.0; extra == "dev"
 Requires-Dist: mypy==1.7.0; extra == "dev"
 Requires-Dist: pre-commit==3.6.1; extra == "dev"
 Requires-Dist: pytest==7.1.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 
-# SoupSavvy
+# soupsavvy
+
+-----------------
+
+## Python package that makes web-scraping more manageable
 
 | | |
 | --- | --- |
 | Package | ![Deployment PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/production_release.yml/badge.svg) ![Deployment test PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/development_release.yml/badge.svg) [![GitHub](https://img.shields.io/badge/GitHub-sewcio543-181717.svg?style=flat&logo=github)](https://github.com/sewcio543) [![PyPI](https://img.shields.io/pypi/v/soupsavvy?color=orange)](https://pypi.org/project/soupsavvy/) [![Python Versions](https://img.shields.io/pypi/pyversions/soupsavvy)](https://www.python.org/)|
 | Testing | ![Tests](https://github.com/sewcio543/soupsavvy/actions/workflows/tests.yml/badge.svg) [![Codecov](https://codecov.io/gh/sewcio543/soupsavvy/graph/badge.svg?token=RZ51VS3QLB)](https://codecov.io/gh/sewcio543/soupsavvy)|
-| Code Quality | ![Build](https://github.com/sewcio543/soupsavvy/actions/workflows/build_package.yml/badge.svg) ![Linting](https://github.com/sewcio543/soupsavvy/actions/workflows/linting.yml/badge.svg) ![Formatting](https://github.com/sewcio543/soupsavvy/actions/workflows/formatting.yml/badge.svg) ![Type Checking](https://github.com/sewcio543/soupsavvy/actions/workflows/type_checking.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sewcio543/soupsavvy/main.svg)](https://results.pre-commit.ci/latest/github/sewcio543/soupsavvy/main)|
+| Code Quality | ![Build](https://github.com/sewcio543/soupsavvy/actions/workflows/build_package.yml/badge.svg) ![Linting](https://github.com/sewcio543/soupsavvy/actions/workflows/linting.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sewcio543/soupsavvy/main.svg)](https://results.pre-commit.ci/latest/github/sewcio543/soupsavvy/main)|
 | Documentation | [![readthedocs](https://img.shields.io/readthedocs/pip?logo=readthedocs)](https://github.com/sewcio543/soupsavvy/actions/workflows/documentation.yml/badge.svg) [![Docs link](https://img.shields.io/badge/docs-check_out-blue)](https://sewcio543.github.io/soupsavvy/)|
 
 ## Table of Contents
 
 - [About](#about)
 - [Key features](#key-features)
 - [Instalation](#installation)
@@ -70,29 +74,29 @@
 - [Contributing](#contributing)
 - [License](#license)
 - [Acknowledgements](#acknowledgements)
 - [In the future](#in-the-future)
 
 ## About
 
-**SoupSavvy** is a library designed to make web scraping tasks more efficient and manageable. Automating web scraping can be a thankless and time-consuming job. SoupSavvy builds around [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) library enabling developers to create more complex workflows and advanced searches with ease.
+**soupsavvy** is a library designed to make web scraping tasks more efficient and manageable. Automating web scraping can be a thankless and time-consuming job. It builds around [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) library enabling developers to create more complex workflows and advanced searches with ease.
 
 ## Key Features
 
-- **Automated Web Scraping**: SoupSavvy simplifies the process of web scraping by providing intuitive interfaces and tools for automating tasks.
+- **Automated Web Scraping**: soupsavvy simplifies the process of web scraping by providing intuitive interfaces and tools for automating tasks.
 
-- **Complex Workflows**: With SoupSavvy, developers can create complex scraping workflows effortlessly, allowing for more intricate data extraction.
+- **Complex Workflows**: With soupsavvy, developers can create complex scraping workflows effortlessly, allowing for more intricate data extraction.
 
-- **Productionalize Scraping Code**: By providing structured workflows and error handling mechanisms, SoupSavvy facilitates the productionalization of scraping code, making it easier to integrate into larger projects and pipelines.
+- **Productionalize Scraping Code**: By providing structured workflows and error handling mechanisms, soupsavvy facilitates the productionalization of scraping code, making it easier to integrate into larger projects and pipelines.
 
 ## Getting Started
 
 ### Installation
 
-SoupSavvy is published on PyPi and can be installed via pip:
+soupsavvy is published on PyPi and can be installed via pip:
 
 ```bash
 pip install soupsavvy
 ```
 
 ### Usage
 
@@ -161,37 +165,37 @@
         re=True,
     ),
 )
 # reuse it in any place to search for tag in any markup, if not found, strict mode raises exception
 a = tag.find(markup, strict=True)
 ```
 
-This streamlined SoupSavvy approach and encapsulating complex tag(s) into single objects transforms web scraping tasks from a potential 'soup sandwich'🥪 into a 'duck soup' 🦆 scenario.
+This streamlined soupsavvy approach and encapsulating complex tag(s) into single objects transforms web scraping tasks from a potential 'soup sandwich'🥪 into a 'duck soup' 🦆 scenario.
 
-With SoupSavvy's robust features, developers can avoid common problems encountered in web scraping, such as exception handling or integration with type checkers.
+With soupsavvy's robust features, developers can avoid common problems encountered in web scraping, such as exception handling or integration with type checkers.
 
-Full documentation can be found at **[Soupsavvy Docs](https://sewcio543.github.io/soupsavvy/)**
+Full documentation can be found at **[soupsavvy Docs](https://sewcio543.github.io/soupsavvy/)**
 
 ## Contributing
 
-If you'd like to contribute to SoupSavvy, feel free to check out the [GitHub repository](https://github.com/sewcio543/soupsavvy) and submit pull requests into one of development branches. Any feedback, bug reports, or feature requests are welcome!
+If you'd like to contribute to soupsavvy, feel free to check out the [GitHub repository](https://github.com/sewcio543/soupsavvy) and submit pull requests into one of development branches. Any feedback, bug reports, or feature requests are welcome!
 
 ## License
 
 [![MIT License](https://img.shields.io/badge/license-MIT-green?style=plastic)](https://choosealicense.com/licenses/mit/)  
-SoupSavvy is licensed under the [MIT License](https://opensource.org/licenses/MIT), allowing for both personal and commercial use. See the `LICENSE` file for more information.
+soupsavvy is licensed under the [MIT License](https://opensource.org/licenses/MIT), allowing for both personal and commercial use. See the `LICENSE` file for more information.
 
 ## Acknowledgements
 
-SoupSavvy is built upon the foundation of excellent BeautifulSoup. We extend our gratitude to the developers and contributors of this projects for their invaluable contributions to the Python community and making our life a lot easier!
+Soupsavvy is built upon the foundation of excellent BeautifulSoup. We extend our gratitude to the developers and contributors of this projects for their invaluable contributions to the Python community and making our life a lot easier!
 
----
+-----------------
 
-Make your soup more beautiful and savvier!  
-Happy scraping! 🍲✨
+**Let's soap this soup!**  
+**Happy scraping!** ✨
 
 ## In the future
 
 - Scraping workflows from soup to nuts
 - New Tag components
 - Enhanced CI pipeline
 - Documentation
```

### Comparing `soupsavvy-0.1.3/README.md` & `soupsavvy-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-# SoupSavvy
+# soupsavvy
+
+-----------------
+
+## Python package that makes web-scraping more manageable
 
 | | |
 | --- | --- |
 | Package | ![Deployment PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/production_release.yml/badge.svg) ![Deployment test PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/development_release.yml/badge.svg) [![GitHub](https://img.shields.io/badge/GitHub-sewcio543-181717.svg?style=flat&logo=github)](https://github.com/sewcio543) [![PyPI](https://img.shields.io/pypi/v/soupsavvy?color=orange)](https://pypi.org/project/soupsavvy/) [![Python Versions](https://img.shields.io/pypi/pyversions/soupsavvy)](https://www.python.org/)|
 | Testing | ![Tests](https://github.com/sewcio543/soupsavvy/actions/workflows/tests.yml/badge.svg) [![Codecov](https://codecov.io/gh/sewcio543/soupsavvy/graph/badge.svg?token=RZ51VS3QLB)](https://codecov.io/gh/sewcio543/soupsavvy)|
-| Code Quality | ![Build](https://github.com/sewcio543/soupsavvy/actions/workflows/build_package.yml/badge.svg) ![Linting](https://github.com/sewcio543/soupsavvy/actions/workflows/linting.yml/badge.svg) ![Formatting](https://github.com/sewcio543/soupsavvy/actions/workflows/formatting.yml/badge.svg) ![Type Checking](https://github.com/sewcio543/soupsavvy/actions/workflows/type_checking.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sewcio543/soupsavvy/main.svg)](https://results.pre-commit.ci/latest/github/sewcio543/soupsavvy/main)|
+| Code Quality | ![Build](https://github.com/sewcio543/soupsavvy/actions/workflows/build_package.yml/badge.svg) ![Linting](https://github.com/sewcio543/soupsavvy/actions/workflows/linting.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sewcio543/soupsavvy/main.svg)](https://results.pre-commit.ci/latest/github/sewcio543/soupsavvy/main)|
 | Documentation | [![readthedocs](https://img.shields.io/readthedocs/pip?logo=readthedocs)](https://github.com/sewcio543/soupsavvy/actions/workflows/documentation.yml/badge.svg) [![Docs link](https://img.shields.io/badge/docs-check_out-blue)](https://sewcio543.github.io/soupsavvy/)|
 
 ## Table of Contents
 
 - [About](#about)
 - [Key features](#key-features)
 - [Instalation](#installation)
@@ -16,29 +20,29 @@
 - [Contributing](#contributing)
 - [License](#license)
 - [Acknowledgements](#acknowledgements)
 - [In the future](#in-the-future)
 
 ## About
 
-**SoupSavvy** is a library designed to make web scraping tasks more efficient and manageable. Automating web scraping can be a thankless and time-consuming job. SoupSavvy builds around [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) library enabling developers to create more complex workflows and advanced searches with ease.
+**soupsavvy** is a library designed to make web scraping tasks more efficient and manageable. Automating web scraping can be a thankless and time-consuming job. It builds around [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) library enabling developers to create more complex workflows and advanced searches with ease.
 
 ## Key Features
 
-- **Automated Web Scraping**: SoupSavvy simplifies the process of web scraping by providing intuitive interfaces and tools for automating tasks.
+- **Automated Web Scraping**: soupsavvy simplifies the process of web scraping by providing intuitive interfaces and tools for automating tasks.
 
-- **Complex Workflows**: With SoupSavvy, developers can create complex scraping workflows effortlessly, allowing for more intricate data extraction.
+- **Complex Workflows**: With soupsavvy, developers can create complex scraping workflows effortlessly, allowing for more intricate data extraction.
 
-- **Productionalize Scraping Code**: By providing structured workflows and error handling mechanisms, SoupSavvy facilitates the productionalization of scraping code, making it easier to integrate into larger projects and pipelines.
+- **Productionalize Scraping Code**: By providing structured workflows and error handling mechanisms, soupsavvy facilitates the productionalization of scraping code, making it easier to integrate into larger projects and pipelines.
 
 ## Getting Started
 
 ### Installation
 
-SoupSavvy is published on PyPi and can be installed via pip:
+soupsavvy is published on PyPi and can be installed via pip:
 
 ```bash
 pip install soupsavvy
 ```
 
 ### Usage
 
@@ -107,37 +111,37 @@
         re=True,
     ),
 )
 # reuse it in any place to search for tag in any markup, if not found, strict mode raises exception
 a = tag.find(markup, strict=True)
 ```
 
-This streamlined SoupSavvy approach and encapsulating complex tag(s) into single objects transforms web scraping tasks from a potential 'soup sandwich'🥪 into a 'duck soup' 🦆 scenario.
+This streamlined soupsavvy approach and encapsulating complex tag(s) into single objects transforms web scraping tasks from a potential 'soup sandwich'🥪 into a 'duck soup' 🦆 scenario.
 
-With SoupSavvy's robust features, developers can avoid common problems encountered in web scraping, such as exception handling or integration with type checkers.
+With soupsavvy's robust features, developers can avoid common problems encountered in web scraping, such as exception handling or integration with type checkers.
 
-Full documentation can be found at **[Soupsavvy Docs](https://sewcio543.github.io/soupsavvy/)**
+Full documentation can be found at **[soupsavvy Docs](https://sewcio543.github.io/soupsavvy/)**
 
 ## Contributing
 
-If you'd like to contribute to SoupSavvy, feel free to check out the [GitHub repository](https://github.com/sewcio543/soupsavvy) and submit pull requests into one of development branches. Any feedback, bug reports, or feature requests are welcome!
+If you'd like to contribute to soupsavvy, feel free to check out the [GitHub repository](https://github.com/sewcio543/soupsavvy) and submit pull requests into one of development branches. Any feedback, bug reports, or feature requests are welcome!
 
 ## License
 
 [![MIT License](https://img.shields.io/badge/license-MIT-green?style=plastic)](https://choosealicense.com/licenses/mit/)  
-SoupSavvy is licensed under the [MIT License](https://opensource.org/licenses/MIT), allowing for both personal and commercial use. See the `LICENSE` file for more information.
+soupsavvy is licensed under the [MIT License](https://opensource.org/licenses/MIT), allowing for both personal and commercial use. See the `LICENSE` file for more information.
 
 ## Acknowledgements
 
-SoupSavvy is built upon the foundation of excellent BeautifulSoup. We extend our gratitude to the developers and contributors of this projects for their invaluable contributions to the Python community and making our life a lot easier!
+Soupsavvy is built upon the foundation of excellent BeautifulSoup. We extend our gratitude to the developers and contributors of this projects for their invaluable contributions to the Python community and making our life a lot easier!
 
----
+-----------------
 
-Make your soup more beautiful and savvier!  
-Happy scraping! 🍲✨
+**Let's soap this soup!**  
+**Happy scraping!** ✨
 
 ## In the future
 
 - Scraping workflows from soup to nuts
 - New Tag components
 - Enhanced CI pipeline
 - Documentation
```

### Comparing `soupsavvy-0.1.3/pyproject.toml` & `soupsavvy-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version", "dependencies", "optional-dependencies"]
 
 [tool.setuptools.dynamic]
 version = {attr = "soupsavvy.__version__"}
 dependencies = {file = ["requirements.txt"]}
-optional-dependencies = {dev = { file = ["config/requirements_dev.txt"] }}
+optional-dependencies = {dev = { file = ["requirements_dev.txt"] }}
 
 [tool.setuptools]
 packages = ["soupsavvy"]
 
 [project.urls]
 source = "https://github.com/sewcio543/soupsavvy"
```

### Comparing `soupsavvy-0.1.3/soupsavvy.egg-info/PKG-INFO` & `soupsavvy-0.1.4/soupsavvy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soupsavvy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python package for advanced web scraping
 Author: sewcio543
 License: MIT License
         
         Copyright (c) 2024 Wojciech Seweryn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,32 +37,36 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.2
 Requires-Dist: lxml==4.9.2
 Provides-Extra: dev
-Requires-Dist: black==24.1.1; extra == "dev"
+Requires-Dist: black==24.3.0; extra == "dev"
 Requires-Dist: build==1.0.3; extra == "dev"
 Requires-Dist: bump2version==1.0.1; extra == "dev"
 Requires-Dist: codecov==2.1.13; extra == "dev"
 Requires-Dist: coverage==7.2.2; extra == "dev"
 Requires-Dist: flake8==7.0.0; extra == "dev"
 Requires-Dist: mypy==1.7.0; extra == "dev"
 Requires-Dist: pre-commit==3.6.1; extra == "dev"
 Requires-Dist: pytest==7.1.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 
-# SoupSavvy
+# soupsavvy
+
+-----------------
+
+## Python package that makes web-scraping more manageable
 
 | | |
 | --- | --- |
 | Package | ![Deployment PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/production_release.yml/badge.svg) ![Deployment test PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/development_release.yml/badge.svg) [![GitHub](https://img.shields.io/badge/GitHub-sewcio543-181717.svg?style=flat&logo=github)](https://github.com/sewcio543) [![PyPI](https://img.shields.io/pypi/v/soupsavvy?color=orange)](https://pypi.org/project/soupsavvy/) [![Python Versions](https://img.shields.io/pypi/pyversions/soupsavvy)](https://www.python.org/)|
 | Testing | ![Tests](https://github.com/sewcio543/soupsavvy/actions/workflows/tests.yml/badge.svg) [![Codecov](https://codecov.io/gh/sewcio543/soupsavvy/graph/badge.svg?token=RZ51VS3QLB)](https://codecov.io/gh/sewcio543/soupsavvy)|
-| Code Quality | ![Build](https://github.com/sewcio543/soupsavvy/actions/workflows/build_package.yml/badge.svg) ![Linting](https://github.com/sewcio543/soupsavvy/actions/workflows/linting.yml/badge.svg) ![Formatting](https://github.com/sewcio543/soupsavvy/actions/workflows/formatting.yml/badge.svg) ![Type Checking](https://github.com/sewcio543/soupsavvy/actions/workflows/type_checking.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sewcio543/soupsavvy/main.svg)](https://results.pre-commit.ci/latest/github/sewcio543/soupsavvy/main)|
+| Code Quality | ![Build](https://github.com/sewcio543/soupsavvy/actions/workflows/build_package.yml/badge.svg) ![Linting](https://github.com/sewcio543/soupsavvy/actions/workflows/linting.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sewcio543/soupsavvy/main.svg)](https://results.pre-commit.ci/latest/github/sewcio543/soupsavvy/main)|
 | Documentation | [![readthedocs](https://img.shields.io/readthedocs/pip?logo=readthedocs)](https://github.com/sewcio543/soupsavvy/actions/workflows/documentation.yml/badge.svg) [![Docs link](https://img.shields.io/badge/docs-check_out-blue)](https://sewcio543.github.io/soupsavvy/)|
 
 ## Table of Contents
 
 - [About](#about)
 - [Key features](#key-features)
 - [Instalation](#installation)
@@ -70,29 +74,29 @@
 - [Contributing](#contributing)
 - [License](#license)
 - [Acknowledgements](#acknowledgements)
 - [In the future](#in-the-future)
 
 ## About
 
-**SoupSavvy** is a library designed to make web scraping tasks more efficient and manageable. Automating web scraping can be a thankless and time-consuming job. SoupSavvy builds around [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) library enabling developers to create more complex workflows and advanced searches with ease.
+**soupsavvy** is a library designed to make web scraping tasks more efficient and manageable. Automating web scraping can be a thankless and time-consuming job. It builds around [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) library enabling developers to create more complex workflows and advanced searches with ease.
 
 ## Key Features
 
-- **Automated Web Scraping**: SoupSavvy simplifies the process of web scraping by providing intuitive interfaces and tools for automating tasks.
+- **Automated Web Scraping**: soupsavvy simplifies the process of web scraping by providing intuitive interfaces and tools for automating tasks.
 
-- **Complex Workflows**: With SoupSavvy, developers can create complex scraping workflows effortlessly, allowing for more intricate data extraction.
+- **Complex Workflows**: With soupsavvy, developers can create complex scraping workflows effortlessly, allowing for more intricate data extraction.
 
-- **Productionalize Scraping Code**: By providing structured workflows and error handling mechanisms, SoupSavvy facilitates the productionalization of scraping code, making it easier to integrate into larger projects and pipelines.
+- **Productionalize Scraping Code**: By providing structured workflows and error handling mechanisms, soupsavvy facilitates the productionalization of scraping code, making it easier to integrate into larger projects and pipelines.
 
 ## Getting Started
 
 ### Installation
 
-SoupSavvy is published on PyPi and can be installed via pip:
+soupsavvy is published on PyPi and can be installed via pip:
 
 ```bash
 pip install soupsavvy
 ```
 
 ### Usage
 
@@ -161,37 +165,37 @@
         re=True,
     ),
 )
 # reuse it in any place to search for tag in any markup, if not found, strict mode raises exception
 a = tag.find(markup, strict=True)
 ```
 
-This streamlined SoupSavvy approach and encapsulating complex tag(s) into single objects transforms web scraping tasks from a potential 'soup sandwich'🥪 into a 'duck soup' 🦆 scenario.
+This streamlined soupsavvy approach and encapsulating complex tag(s) into single objects transforms web scraping tasks from a potential 'soup sandwich'🥪 into a 'duck soup' 🦆 scenario.
 
-With SoupSavvy's robust features, developers can avoid common problems encountered in web scraping, such as exception handling or integration with type checkers.
+With soupsavvy's robust features, developers can avoid common problems encountered in web scraping, such as exception handling or integration with type checkers.
 
-Full documentation can be found at **[Soupsavvy Docs](https://sewcio543.github.io/soupsavvy/)**
+Full documentation can be found at **[soupsavvy Docs](https://sewcio543.github.io/soupsavvy/)**
 
 ## Contributing
 
-If you'd like to contribute to SoupSavvy, feel free to check out the [GitHub repository](https://github.com/sewcio543/soupsavvy) and submit pull requests into one of development branches. Any feedback, bug reports, or feature requests are welcome!
+If you'd like to contribute to soupsavvy, feel free to check out the [GitHub repository](https://github.com/sewcio543/soupsavvy) and submit pull requests into one of development branches. Any feedback, bug reports, or feature requests are welcome!
 
 ## License
 
 [![MIT License](https://img.shields.io/badge/license-MIT-green?style=plastic)](https://choosealicense.com/licenses/mit/)  
-SoupSavvy is licensed under the [MIT License](https://opensource.org/licenses/MIT), allowing for both personal and commercial use. See the `LICENSE` file for more information.
+soupsavvy is licensed under the [MIT License](https://opensource.org/licenses/MIT), allowing for both personal and commercial use. See the `LICENSE` file for more information.
 
 ## Acknowledgements
 
-SoupSavvy is built upon the foundation of excellent BeautifulSoup. We extend our gratitude to the developers and contributors of this projects for their invaluable contributions to the Python community and making our life a lot easier!
+Soupsavvy is built upon the foundation of excellent BeautifulSoup. We extend our gratitude to the developers and contributors of this projects for their invaluable contributions to the Python community and making our life a lot easier!
 
----
+-----------------
 
-Make your soup more beautiful and savvier!  
-Happy scraping! 🍲✨
+**Let's soap this soup!**  
+**Happy scraping!** ✨
 
 ## In the future
 
 - Scraping workflows from soup to nuts
 - New Tag components
 - Enhanced CI pipeline
 - Documentation
```

