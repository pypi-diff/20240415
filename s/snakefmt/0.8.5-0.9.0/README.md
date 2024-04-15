# Comparing `tmp/snakefmt-0.8.5.tar.gz` & `tmp/snakefmt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakefmt-0.8.5.tar", max compression
+gzip compressed data, was "snakefmt-0.9.0.tar", max compression
```

## Comparing `snakefmt-0.8.5.tar` & `snakefmt-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1087 2023-10-05 02:15:48.234765 snakefmt-0.8.5/LICENSE
--rw-r--r--   0        0        0    12739 2023-10-05 02:15:48.238765 snakefmt-0.8.5/README.md
--rw-r--r--   0        0        0     1458 2023-10-05 02:15:48.238765 snakefmt-0.8.5/pyproject.toml
--rw-r--r--   0        0        0      423 2023-10-05 02:15:48.238765 snakefmt-0.8.5/snakefmt/__init__.py
--rw-r--r--   0        0        0      100 2023-10-05 02:15:48.238765 snakefmt-0.8.5/snakefmt/__main__.py
--rw-r--r--   0        0        0     2805 2023-10-05 02:15:48.238765 snakefmt-0.8.5/snakefmt/config.py
--rw-r--r--   0        0        0     1014 2023-10-05 02:15:48.238765 snakefmt-0.8.5/snakefmt/diff.py
--rw-r--r--   0        0        0     1133 2023-10-05 02:15:48.238765 snakefmt-0.8.5/snakefmt/exceptions.py
--rw-r--r--   0        0        0    15819 2023-10-05 02:15:48.238765 snakefmt-0.8.5/snakefmt/formatter.py
--rw-r--r--   0        0        0     1522 2023-10-05 02:15:48.238765 snakefmt-0.8.5/snakefmt/logging.py
--rw-r--r--   0        0        0     3849 2023-10-05 02:15:48.238765 snakefmt-0.8.5/snakefmt/parser/grammar.py
--rw-r--r--   0        0        0    12133 2023-10-05 02:15:48.238765 snakefmt-0.8.5/snakefmt/parser/parser.py
--rw-r--r--   0        0        0    14861 2023-10-05 02:15:48.238765 snakefmt-0.8.5/snakefmt/parser/syntax.py
--rw-r--r--   0        0        0    10162 2023-10-05 02:15:48.238765 snakefmt-0.8.5/snakefmt/snakefmt.py
--rw-r--r--   0        0        0      570 2023-10-05 02:15:48.238765 snakefmt-0.8.5/snakefmt/types.py
--rw-r--r--   0        0        0    14132 1970-01-01 00:00:00.000000 snakefmt-0.8.5/setup.py
--rw-r--r--   0        0        0    13952 1970-01-01 00:00:00.000000 snakefmt-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-01-09 11:46:03.186473 snakefmt-0.9.0/LICENSE
+-rw-r--r--   0        0        0    12739 2024-01-09 11:46:03.186473 snakefmt-0.9.0/README.md
+-rw-r--r--   0        0        0     1456 2024-01-09 11:46:03.186473 snakefmt-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      423 2024-01-09 11:46:03.186473 snakefmt-0.9.0/snakefmt/__init__.py
+-rw-r--r--   0        0        0      100 2024-01-09 11:46:03.186473 snakefmt-0.9.0/snakefmt/__main__.py
+-rw-r--r--   0        0        0     2805 2024-01-09 11:46:03.186473 snakefmt-0.9.0/snakefmt/config.py
+-rw-r--r--   0        0        0     1014 2024-01-09 11:46:03.186473 snakefmt-0.9.0/snakefmt/diff.py
+-rw-r--r--   0        0        0     1133 2024-01-09 11:46:03.186473 snakefmt-0.9.0/snakefmt/exceptions.py
+-rw-r--r--   0        0        0    16093 2024-01-09 11:46:03.186473 snakefmt-0.9.0/snakefmt/formatter.py
+-rw-r--r--   0        0        0     1522 2024-01-09 11:46:03.186473 snakefmt-0.9.0/snakefmt/logging.py
+-rw-r--r--   0        0        0     3849 2024-01-09 11:46:03.186473 snakefmt-0.9.0/snakefmt/parser/grammar.py
+-rw-r--r--   0        0        0    12133 2024-01-09 11:46:03.186473 snakefmt-0.9.0/snakefmt/parser/parser.py
+-rw-r--r--   0        0        0    15564 2024-01-09 11:46:03.186473 snakefmt-0.9.0/snakefmt/parser/syntax.py
+-rw-r--r--   0        0        0    10162 2024-01-09 11:46:03.186473 snakefmt-0.9.0/snakefmt/snakefmt.py
+-rw-r--r--   0        0        0      570 2024-01-09 11:46:03.186473 snakefmt-0.9.0/snakefmt/types.py
+-rw-r--r--   0        0        0    13904 1970-01-01 00:00:00.000000 snakefmt-0.9.0/PKG-INFO
```

### Comparing `snakefmt-0.8.5/LICENSE` & `snakefmt-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snakefmt-0.8.5/README.md` & `snakefmt-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `snakefmt-0.8.5/pyproject.toml` & `snakefmt-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "snakefmt"
-version = "0.8.5"
+version = "0.9.0"
 description = "The uncompromising Snakemake code formatter"
 authors = ["Michael Hall <michael@mbh.sh>", "Brice Letcher <bletcher@ebi.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/snakemake/snakefmt"
 repository = "https://github.com/snakemake/snakefmt"
 documentation = "https://github.com/snakemake/snakefmt/blob/master/README.md"
 keywords = ["python", "snakemake", "code", "formatter", "parser", "workflow", "management", "systems", "black"]
 
 [tool.poetry.scripts]
 snakefmt = 'snakefmt.snakefmt:main'
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
+python = "^3.8.1"
 click = "^8.0.0"
-black = "^23.1.0"
+black = "^23.12.1"
 toml = "^0.10.2"
 importlib_metadata = {version = ">=1.7.0,<5.0", python = "<3.8"}
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-pytest-cov = "^2.8.1"
-flake8 = "^3.7.9"
-snakemake = "^7.11"
+pytest = "^7.4.4"
+pytest-cov = "^4.1.0"
+flake8 = "^7.0"
+snakemake = "<8.0"
 isort = "^5.1.0"
 pynvim = "~0.4.3"
 
 [tool.poetry.urls]
 "Snakemake Documentation" = "https://snakemake.readthedocs.io/"
 "Snakemake Repository" = "https://github.com/snakemake/snakemake"
```

### Comparing `snakefmt-0.8.5/snakefmt/config.py` & `snakefmt-0.9.0/snakefmt/config.py`

 * *Files identical despite different names*

### Comparing `snakefmt-0.8.5/snakefmt/diff.py` & `snakefmt-0.9.0/snakefmt/diff.py`

 * *Files identical despite different names*

### Comparing `snakefmt-0.8.5/snakefmt/exceptions.py` & `snakefmt-0.9.0/snakefmt/exceptions.py`

 * *Files identical despite different names*

### Comparing `snakefmt-0.8.5/snakefmt/formatter.py` & `snakefmt-0.9.0/snakefmt/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,52 +215,58 @@
         """
         pos = 0
         used_indent = TAB * target_indent
         indented = ""
         for match in re.finditer(full_string_matcher, string):
             indented += textwrap.indent(string[pos : match.start(1)], used_indent)
             lagging_spaces = len(indented) - len(indented.rstrip(" "))
-            lagging_indent = (
-                TAB * int(lagging_spaces / TAB_SIZE)
-                if lagging_spaces % TAB_SIZE == 0
-                else ""
-            )
+            lagging_indent_lvl = lagging_spaces // TAB_SIZE
             match_slice = string[match.start(1) : match.end(1)].replace("\t", TAB)
             all_lines = match_slice.splitlines(keepends=True)
             first = textwrap.indent(textwrap.dedent(all_lines[0]), used_indent)
+            indented += first
+
             is_multiline_string = re.match(
                 r"[bfru]?\"\"\"|'''", first.lstrip(), flags=re.IGNORECASE
             )
-            indented += first
+            if not is_multiline_string:
+                # this check if string is a single-quoted multiline string
+                # e.g. https://github.com/snakemake/snakefmt/issues/121
+                is_multiline_string = "\\\n" in first
 
             if len(all_lines) > 2:
                 if is_multiline_string:
                     middle = "".join(all_lines[1:-1])
                 else:
                     mid = "".join(all_lines[1:-1])
                     dedent_mid = textwrap.dedent(mid)
-                    lagging_indent_lvl = lagging_spaces // TAB_SIZE
+
                     if lagging_indent_lvl == 0:
                         required_indent_lvl = target_indent
                     else:
                         current_indent_lvl = (len(mid) - len(mid.lstrip())) // TAB_SIZE
                         required_indent_lvl = current_indent_lvl + target_indent
 
                     required_indent = TAB * required_indent_lvl
                     middle = textwrap.indent(
                         dedent_mid,
                         required_indent,
                     )
                 indented += middle
+
             if len(all_lines) > 1:
                 if is_multiline_string:
                     last = all_lines[-1]
                 else:
+                    leading_spaces = len(all_lines[-1]) - len(
+                        textwrap.dedent(all_lines[-1])
+                    )
+                    leading_indent = leading_spaces // TAB_SIZE * TAB
                     last = textwrap.indent(
-                        textwrap.dedent(all_lines[-1]), used_indent + lagging_indent
+                        textwrap.dedent(all_lines[-1]), used_indent + leading_indent
                     )
                 indented += last
             pos = match.end()
         indented += textwrap.indent(string[pos:], used_indent)
 
         return indented
```

### Comparing `snakefmt-0.8.5/snakefmt/logging.py` & `snakefmt-0.9.0/snakefmt/logging.py`

 * *Files identical despite different names*

### Comparing `snakefmt-0.8.5/snakefmt/parser/grammar.py` & `snakefmt-0.9.0/snakefmt/parser/grammar.py`

 * *Files identical despite different names*

### Comparing `snakefmt-0.8.5/snakefmt/parser/parser.py` & `snakefmt-0.9.0/snakefmt/parser/parser.py`

 * *Files identical despite different names*

### Comparing `snakefmt-0.8.5/snakefmt/parser/syntax.py` & `snakefmt-0.9.0/snakefmt/parser/syntax.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Code in charge of parsing and validating Snakemake syntax
 """
+import sys
 import tokenize
 from abc import ABC, abstractmethod
 from re import match as re_match
 
 from snakefmt.exceptions import (
     ColonError,
     EmptyContextError,
@@ -32,28 +33,34 @@
 # ___Token spacing: for when cannot run black___#
 spacing_triggers = {
     tokenize.NAME: {tokenize.NAME, tokenize.STRING, tokenize.NUMBER, tokenize.OP},
     tokenize.STRING: {tokenize.NAME, tokenize.OP},
     tokenize.NUMBER: {tokenize.NAME, tokenize.OP},
     tokenize.OP: {tokenize.NAME, tokenize.STRING, tokenize.NUMBER, tokenize.OP},
 }
+# add fstring start to spacing_triggers if python 3.12 or higher
+if hasattr(tokenize, "FSTRING_START"):
+    spacing_triggers[tokenize.NAME].add(tokenize.FSTRING_START)
+    spacing_triggers[tokenize.OP].add(tokenize.FSTRING_START)
 
 
 def operator_skip_spacing(prev_token: Token, token: Token) -> bool:
     if prev_token.type != tokenize.OP and token.type != tokenize.OP:
         return False
     if (
         prev_token.string in BRACKETS_OPEN
         or prev_token.string == "."
         or token.string in BRACKETS_CLOSE
         or token.string in {"[", ":", "."}
     ):
         return True
     elif prev_token.type == tokenize.NAME and token.string == "(":
         return True
+    elif prev_token.type == tokenize.STRING and token.string == ",":
+        return True
     else:
         return False
 
 
 def add_token_space(prev_token: Token, token: Token) -> bool:
     result = False
     if prev_token is not None and prev_token.type in spacing_triggers:
@@ -319,17 +326,25 @@
     @property
     def in_brackets(self):
         return len(self._brackets) > 0
 
     def parse_params(self, snakefile: TokenIterator):
         cur_param = Parameter(self.token)
         prev_token = None
-
         while True:
             cur_param = self.process_token(cur_param, prev_token)
+            if (
+                self.token is not None
+                and sys.version_info >= (3, 12)
+                and self.token.type == tokenize.FSTRING_MIDDLE
+            ):
+                if self.token.string.endswith("}"):
+                    cur_param.value += "}"
+                elif self.token.string.endswith("{"):
+                    cur_param.value += "{"
             try:
                 prev_token = self.token
                 self.token = next(snakefile)
             except StopIteration:
                 self.flush_param(cur_param, skip_empty=True)
                 self.eof = True
                 break
```

### Comparing `snakefmt-0.8.5/snakefmt/snakefmt.py` & `snakefmt-0.9.0/snakefmt/snakefmt.py`

 * *Files identical despite different names*

### Comparing `snakefmt-0.8.5/snakefmt/types.py` & `snakefmt-0.9.0/snakefmt/types.py`

 * *Files identical despite different names*

### Comparing `snakefmt-0.8.5/setup.py` & `snakefmt-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,431 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: snakefmt
+Version: 0.9.0
+Summary: The uncompromising Snakemake code formatter
+Home-page: https://github.com/snakemake/snakefmt
+License: MIT
+Keywords: python,snakemake,code,formatter,parser,workflow,management,systems,black
+Author: Michael Hall
+Author-email: michael@mbh.sh
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: black (>=23.12.1,<24.0.0)
+Requires-Dist: click (>=8.0.0,<9.0.0)
+Requires-Dist: importlib_metadata (>=1.7.0,<5.0) ; python_version < "3.8"
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Documentation, https://github.com/snakemake/snakefmt/blob/master/README.md
+Project-URL: Repository, https://github.com/snakemake/snakefmt
+Project-URL: Snakemake Documentation, https://snakemake.readthedocs.io/
+Project-URL: Snakemake Repository, https://github.com/snakemake/snakemake
+Description-Content-Type: text/markdown
 
-packages = \
-['snakefmt', 'snakefmt.parser']
+# Snakefmt
 
-package_data = \
-{'': ['*']}
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/snakemake/snakefmt/ci.yaml?branch=master)
+[![codecov](https://codecov.io/gh/snakemake/snakefmt/branch/master/graph/badge.svg)](https://codecov.io/gh/snakemake/snakefmt)
+[![PyPI](https://img.shields.io/pypi/v/snakefmt)](https://pypi.org/project/snakefmt/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/snakefmt)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-install_requires = \
-['black>=23.1.0,<24.0.0', 'click>=8.0.0,<9.0.0', 'toml>=0.10.2,<0.11.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib_metadata>=1.7.0,<5.0']}
-
-entry_points = \
-{'console_scripts': ['snakefmt = snakefmt.snakefmt:main']}
-
-setup_kwargs = {
-    'name': 'snakefmt',
-    'version': '0.8.5',
-    'description': 'The uncompromising Snakemake code formatter',
-    'long_description': '# Snakefmt\n\n![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/snakemake/snakefmt/ci.yaml?branch=master)\n[![codecov](https://codecov.io/gh/snakemake/snakefmt/branch/master/graph/badge.svg)](https://codecov.io/gh/snakemake/snakefmt)\n[![PyPI](https://img.shields.io/pypi/v/snakefmt)](https://pypi.org/project/snakefmt/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/snakefmt)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nThis repository provides formatting for [Snakemake][snakemake] files. It follows the\ndesign and specifications of [Black][black].\n\n> **⚠️WARNING⚠️**: `snakefmt` modifies files in-place by default, thus we strongly\n> recommend ensuring your files are under version control before doing any formatting.\n> You\n> can also pipe the file in from stdin, which will print it to the screen, or use the\n> `--diff` or `--check` options. See [Usage](#usage) for more details.\n\n[TOC]: #\n\n# Table of Contents\n- [Install](#install)\n  - [PyPi](#pypi)\n  - [Conda](#conda)\n  - [Containers](#containers)\n  - [Local](#local)\n- [Example File](#example-file)\n- [Usage](#usage)\n  - [Basic Usage](#basic-usage)\n  - [Full Usage](#full-usage)\n- [Configuration](#configuration)\n- [Integration](#integration)\n    - [Editor Integration](#editor-integration)\n    - [Version Control Integration](#version-control-integration)\n    - [Github Actions](#github-actions)\n- [Plug Us](#plug-us)\n- [Changes](#changes)\n- [Contributing](#contributing)\n- [Cite](#cite)\n\n\n## Install\n\n### PyPi\n\n```sh\npip install snakefmt\n```\n\n### Conda\n\n[![Conda (channel only)](https://img.shields.io/conda/vn/bioconda/snakefmt)](https://anaconda.org/bioconda/snakefmt)\n[![bioconda version](https://anaconda.org/bioconda/snakefmt/badges/platforms.svg)](https://anaconda.org/bioconda/snakefmt)\n\n```sh\nconda install -c bioconda snakefmt\n```\n\n### Containers\n\nAs `snakefmt` has a Conda recipe, there is a matching image built for each version by\nBiocontainers.\n\nIn the following examples, all tags (`<tag>`) can be found\n[here](https://quay.io/repository/biocontainers/snakefmt?tab=tags).\n\n#### Docker\n\n```shell\n$ docker run -it "quay.io/biocontainers/snakefmt:<tag>" snakefmt --help\n```\n\n#### Singularity\n\n```shell\n$ singularity exec "docker://quay.io/biocontainers/snakefmt:<tag>" snakefmt --help\n```\n\n### Local\n\nThese instructions include [installing `poetry`](https://python-poetry.org/docs/#installation).\n```sh\n# install poetry\ncurl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python3\n\ngit clone https://github.com/snakemake/snakefmt && cd snakefmt\n# install snakefmt in a new environment\npoetry install\n# activate the environment so snakefmt is available on your PATH\npoetry shell\n```\n\n## Example File\n\nInput\n\n```python\nfrom snakemake.utils import min_version\nmin_version("5.14.0")\nconfigfile: "config.yaml" # snakemake keywords are treated like classes i.e. 2 newlines\nSAMPLES = [\'s1\', \'s2\'] # strings are normalised\nCONDITIONS = ["a", "b", "longlonglonglonglonglonglonglonglonglonglonglonglonglonglonglong"] # long lines are wrapped\ninclude: "rules/foo.smk" # 2 newlines\n\nrule all:\n    input: "data/results.txt" # newlines after keywords enforced and trailing comma\n\nrule gets_separated_by_two_newlines:\n    input:\n        files = expand("long/string/to/data/files/gets_broken_by_black/{sample}.{condition}",sample=SAMPLES, condition=CONDITIONS)\nif True:\n    rule can_be_inside_python_code:\n        input: "parameters", "get_indented"\n        threads: 4 # Numeric params stay unindented\n        params: key_val = "PEP8_formatted"\n        run:\n\n                print("weirdly_spaced_string_gets_respaced")\n\n```\n\n\nOutput\n\n```python\nfrom snakemake.utils import min_version\n\nmin_version("5.14.0")\n\n\nconfigfile: "config.yaml" # snakemake keywords are treated like classes i.e. 2 newlines\n\n\nSAMPLES = ["s1", "s2"] # strings are normalised\nCONDITIONS = [\n    "a",\n    "b",\n    "longlonglonglonglonglonglonglonglonglonglonglonglonglonglonglong",\n]  # long lines are wrapped\n\n\ninclude: "rules/foo.smk" # 2 newlines\n\n\nrule all:\n    input:\n        "data/results.txt", # newlines after keywords enforced and trailing comma\n\n\nrule gets_separated_by_two_newlines:\n    input:\n        files=expand(\n            "long/string/to/data/files/gets_broken_by_black/{sample}.{condition}",\n            sample=SAMPLES,\n            condition=CONDITIONS,\n        ),\n\n\nif True:\n\n    rule can_be_inside_python_code:\n        input:\n            "parameters",\n            "get_indented",\n        threads: 4 # Numeric params stay unindented\n        params:\n            key_val="PEP8_formatted",\n        run:\n            print("weirdly_spaced_string_gets_respaced")\n\n```\n\n\n## Usage\n\n### Basic Usage\n\nFormat a single Snakefile.\n\n```shell\nsnakefmt Snakefile\n```\n\nFormat all Snakefiles within a directory.\n\n```shell\nsnakefmt workflows/\n```\n\nFormat a file but write the output to stdout.\n\n```shell\nsnakefmt - < Snakefile\n```\n\n### Full Usage\n\n```\n$ snakefmt --help\nUsage: snakefmt [OPTIONS] [SRC]...\n\n  The uncompromising Snakemake code formatter.\n\n  SRC specifies directories and files to format. Directories will be\n  searched for file names that conform to the include/exclude patterns\n  provided.\n\n  Files are modified in-place by default; use diff, check, or  `snakefmt - <\n  Snakefile` to avoid this.\n\nOptions:\n  -l, --line-length INT  Lines longer than INT will be wrapped.  [default: 88]\n  --check                Don\'t write the files back, just return the status.\n                         Return code 0 means nothing would change. Return code\n                         1 means some files would be reformatted. Return code\n                         123 means there was an error.\n\n  -d, --diff             Don\'t write the files back, just output a diff for\n                         each file to stdout.\n\n  --compact-diff         Same as --diff but only shows lines that would change\n                         plus a few lines of context.\n\n  --include PATTERN      A regular expression that matches files and\n                         directories that should be included on recursive\n                         searches.  An empty value means all files are\n                         included regardless of the name.  Use forward slashes\n                         for directories on all platforms (Windows, too).\n                         Exclusions are calculated first, inclusions later.\n                         [default: (\\.smk$|^Snakefile)]\n\n  --exclude PATTERN      A regular expression that matches files and\n                         directories that should be excluded on recursive\n                         searches.  An empty value means no paths are\n                         excluded. Use forward slashes for directories on all\n                         platforms (Windows, too). Exclusions are calculated\n                         first, inclusions later.  [default: (\\.snakemake|\\.eg\n                         gs|\\.git|\\.hg|\\.mypy_cache|\\.nox|\\.tox|\\.venv|\\.svn|_\n                         build|buck-out|build|dist)]\n\n  -c, --config PATH      Read configuration from PATH. By default, will try to\n                         read from `./pyproject.toml`\n\n  -h, --help             Show this message and exit.\n  -V, --version          Show the version and exit.\n  -v, --verbose          Turns on debug-level logging.\n\n```\n\n## Configuration\n\n`snakefmt` is able to read project-specific default values for its command line options\nfrom a `pyproject.toml` file. In addition, it will also load any [`black`\nconfigurations][black-config] you have in the same file.\n\nBy default, `snakefmt` will search in the parent directories of the formatted file(s)\nfor a file called `pyproject.toml` and use any configuration there.\nIf your configuration file is located somewhere else or called something different,\nspecify it using `--config`.\n\nAny options you pass on the command line will take precedence over default values in the\nconfiguration file.\n\n#### Example\n\n`pyproject.toml`\n\n```toml\n[tool.snakefmt]\nline_length = 90\ninclude = \'\\.smk$|^Snakefile|\\.py$\'\n\n# snakefmt passes these options on to black\n[tool.black]\nskip_string_normalization = true\n```\n\nIn this example we increase the `--line-length` value and also include python (`*.py`)\nfiles for formatting - this effectively runs `black` on them. `snakefmt` will also pass\non the `[tool.black]` settings, internally, to `black`.\n\n\n## Integration\n\n\n### Editor Integration\n\nFor instructions on how to integrate `snakefmt` into your editor of choice, refer to\n[`docs/editor_integration.md`](docs/editor_integration.md)\n\n### Version Control Integration\n\n`snakefmt` supports [pre-commit](https://pre-commit.com/), a framework for managing git pre-commit hooks. Using this framework you can run `snakefmt` whenever you commit a `Snakefile` or `*.smk` file. `Pre-commit` automatically creates an isolated virtual environment with `snakefmt` and will stop the commit if `snakefmt` would modify the file. You then review, stage, and re-commit these changes. Pre-commit is especially useful if you don\'t have access to a CI/CD system like GitHub actions.\n\nTo do so, create the file `.pre-commit-config.yaml` in the root of your project directory with the following:\n\n```yaml\nrepos:\n  - repo: https://github.com/snakemake/snakefmt\n    rev: 0.5.0 # Replace by any tag/version ≥0.2.4 : https://github.com/snakemake/snakefmt/releases\n    hooks:\n      - id: snakefmt\n```\n\nThen [install pre-commit](https://pre-commit.com/#installation) and initialize the pre-commit hooks by running `pre-commit install` (Note you need to run this step once per clone of your repository). Additional pre-commit hooks can be found [here](https://pre-commit.com/hooks.html).\n\n### GitHub Actions\n\n[GitHub Actions](https://github.com/features/actions) in combination with [super-linter](https://github.com/github/super-linter) allows you to automatically run `snakefmt` on all Snakefiles in your repository e.g. whenever you push a new commit.\n\nTo do so, create the file `.github/workflows/linter.yml` in your repository:\n```yaml\n---\nname: Lint Code Base\n\non:\n  push:\n  pull_request:\n    branches: [master]\n\njobs:\n  build:\n    name: Lint Code Base\n    runs-on: ubuntu-latest\n\n    steps:\n      - name: Checkout Code\n        uses: actions/checkout@v2\n\n      - name: Lint Code Base\n        uses: github/super-linter@v3\n        env:\n          VALIDATE_ALL_CODEBASE: false\n          DEFAULT_BRANCH: master\n          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}\n\n          VALIDATE_SNAKEMAKE_SNAKEFMT: true\n```\n\nAdditional configuration parameters can be specified by creating `.github/linters/.snakefmt.toml`:\n```toml\n[tool.black]\nskip_string_normalization = true\n```\n\nFor more information check the `super-linter` readme.\n\n## Plug Us\n\nIf you can\'t get enough of badges, then feel free to show others you\'re using `snakefmt`\nin your project.\n\n[![Code style: snakefmt](https://img.shields.io/badge/code%20style-snakefmt-000000.svg)](https://github.com/snakemake/snakefmt)\n\n#### Markdown\n\n```md\n[![Code style: snakefmt](https://img.shields.io/badge/code%20style-snakefmt-000000.svg)](https://github.com/snakemake/snakefmt)\n```\n\n#### ReStructuredText\n\n```rst\n.. image:: https://img.shields.io/badge/code%20style-snakefmt-000000.svg\n    :target: https://github.com/snakemake/snakefmt\n```\n\n## Changes\n\nSee [`CHANGELOG.md`][changes].\n\n## Contributing\n\nSee [CONTRIBUTING.md][contributing].\n\n## Cite\n\n[![DOI][doi-shield]][doi]\n\n```Bibtex\n@article{snakemake2021,\n  doi = {10.12688/f1000research.29032.2},\n  url = {https://doi.org/10.12688/f1000research.29032.2},\n  year = {2021},\n  month = apr,\n  publisher = {F1000 Research Ltd},\n  volume = {10},\n  pages = {33},\n  author = {Felix M\\"{o}lder and Kim Philipp Jablonski and Brice Letcher and Michael B. Hall and Christopher H. Tomkins-Tinch and Vanessa Sochat and Jan Forster and Soohyun Lee and Sven O. Twardziok and Alexander Kanitz and Andreas Wilm and Manuel Holtgrewe and Sven Rahmann and Sven Nahnsen and Johannes K\\"{o}ster},\n  title = {Sustainable data analysis with Snakemake},\n  journal = {F1000Research}\n}\n```\n\n\n[snakemake]: https://snakemake.readthedocs.io/\n[black]: https://black.readthedocs.io/en/stable/\n[black-config]: https://github.com/psf/black#pyprojecttoml\n[pyproject]: https://github.com/snakemake/snakefmt/blob/master/pyproject.toml\n[poetry]: https://python-poetry.org\n[contributing]: CONTRIBUTING.md\n[changes]: CHANGELOG.md\n[doi-shield]: https://img.shields.io/badge/DOI-10.12688%2Ff1000research.29032.2-brightgreen.svg\n[doi]: https://doi.org/10.12688/f1000research.29032.2\n',
-    'author': 'Michael Hall',
-    'author_email': 'michael@mbh.sh',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/snakemake/snakefmt',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.0,<4.0.0',
+This repository provides formatting for [Snakemake][snakemake] files. It follows the
+design and specifications of [Black][black].
+
+> **⚠️WARNING⚠️**: `snakefmt` modifies files in-place by default, thus we strongly
+> recommend ensuring your files are under version control before doing any formatting.
+> You
+> can also pipe the file in from stdin, which will print it to the screen, or use the
+> `--diff` or `--check` options. See [Usage](#usage) for more details.
+
+[TOC]: #
+
+# Table of Contents
+- [Install](#install)
+  - [PyPi](#pypi)
+  - [Conda](#conda)
+  - [Containers](#containers)
+  - [Local](#local)
+- [Example File](#example-file)
+- [Usage](#usage)
+  - [Basic Usage](#basic-usage)
+  - [Full Usage](#full-usage)
+- [Configuration](#configuration)
+- [Integration](#integration)
+    - [Editor Integration](#editor-integration)
+    - [Version Control Integration](#version-control-integration)
+    - [Github Actions](#github-actions)
+- [Plug Us](#plug-us)
+- [Changes](#changes)
+- [Contributing](#contributing)
+- [Cite](#cite)
+
+
+## Install
+
+### PyPi
+
+```sh
+pip install snakefmt
+```
+
+### Conda
+
+[![Conda (channel only)](https://img.shields.io/conda/vn/bioconda/snakefmt)](https://anaconda.org/bioconda/snakefmt)
+[![bioconda version](https://anaconda.org/bioconda/snakefmt/badges/platforms.svg)](https://anaconda.org/bioconda/snakefmt)
+
+```sh
+conda install -c bioconda snakefmt
+```
+
+### Containers
+
+As `snakefmt` has a Conda recipe, there is a matching image built for each version by
+Biocontainers.
+
+In the following examples, all tags (`<tag>`) can be found
+[here](https://quay.io/repository/biocontainers/snakefmt?tab=tags).
+
+#### Docker
+
+```shell
+$ docker run -it "quay.io/biocontainers/snakefmt:<tag>" snakefmt --help
+```
+
+#### Singularity
+
+```shell
+$ singularity exec "docker://quay.io/biocontainers/snakefmt:<tag>" snakefmt --help
+```
+
+### Local
+
+These instructions include [installing `poetry`](https://python-poetry.org/docs/#installation).
+```sh
+# install poetry
+curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python3
+
+git clone https://github.com/snakemake/snakefmt && cd snakefmt
+# install snakefmt in a new environment
+poetry install
+# activate the environment so snakefmt is available on your PATH
+poetry shell
+```
+
+## Example File
+
+Input
+
+```python
+from snakemake.utils import min_version
+min_version("5.14.0")
+configfile: "config.yaml" # snakemake keywords are treated like classes i.e. 2 newlines
+SAMPLES = ['s1', 's2'] # strings are normalised
+CONDITIONS = ["a", "b", "longlonglonglonglonglonglonglonglonglonglonglonglonglonglonglong"] # long lines are wrapped
+include: "rules/foo.smk" # 2 newlines
+
+rule all:
+    input: "data/results.txt" # newlines after keywords enforced and trailing comma
+
+rule gets_separated_by_two_newlines:
+    input:
+        files = expand("long/string/to/data/files/gets_broken_by_black/{sample}.{condition}",sample=SAMPLES, condition=CONDITIONS)
+if True:
+    rule can_be_inside_python_code:
+        input: "parameters", "get_indented"
+        threads: 4 # Numeric params stay unindented
+        params: key_val = "PEP8_formatted"
+        run:
+
+                print("weirdly_spaced_string_gets_respaced")
+
+```
+
+
+Output
+
+```python
+from snakemake.utils import min_version
+
+min_version("5.14.0")
+
+
+configfile: "config.yaml" # snakemake keywords are treated like classes i.e. 2 newlines
+
+
+SAMPLES = ["s1", "s2"] # strings are normalised
+CONDITIONS = [
+    "a",
+    "b",
+    "longlonglonglonglonglonglonglonglonglonglonglonglonglonglonglong",
+]  # long lines are wrapped
+
+
+include: "rules/foo.smk" # 2 newlines
+
+
+rule all:
+    input:
+        "data/results.txt", # newlines after keywords enforced and trailing comma
+
+
+rule gets_separated_by_two_newlines:
+    input:
+        files=expand(
+            "long/string/to/data/files/gets_broken_by_black/{sample}.{condition}",
+            sample=SAMPLES,
+            condition=CONDITIONS,
+        ),
+
+
+if True:
+
+    rule can_be_inside_python_code:
+        input:
+            "parameters",
+            "get_indented",
+        threads: 4 # Numeric params stay unindented
+        params:
+            key_val="PEP8_formatted",
+        run:
+            print("weirdly_spaced_string_gets_respaced")
+
+```
+
+
+## Usage
+
+### Basic Usage
+
+Format a single Snakefile.
+
+```shell
+snakefmt Snakefile
+```
+
+Format all Snakefiles within a directory.
+
+```shell
+snakefmt workflows/
+```
+
+Format a file but write the output to stdout.
+
+```shell
+snakefmt - < Snakefile
+```
+
+### Full Usage
+
+```
+$ snakefmt --help
+Usage: snakefmt [OPTIONS] [SRC]...
+
+  The uncompromising Snakemake code formatter.
+
+  SRC specifies directories and files to format. Directories will be
+  searched for file names that conform to the include/exclude patterns
+  provided.
+
+  Files are modified in-place by default; use diff, check, or  `snakefmt - <
+  Snakefile` to avoid this.
+
+Options:
+  -l, --line-length INT  Lines longer than INT will be wrapped.  [default: 88]
+  --check                Don't write the files back, just return the status.
+                         Return code 0 means nothing would change. Return code
+                         1 means some files would be reformatted. Return code
+                         123 means there was an error.
+
+  -d, --diff             Don't write the files back, just output a diff for
+                         each file to stdout.
+
+  --compact-diff         Same as --diff but only shows lines that would change
+                         plus a few lines of context.
+
+  --include PATTERN      A regular expression that matches files and
+                         directories that should be included on recursive
+                         searches.  An empty value means all files are
+                         included regardless of the name.  Use forward slashes
+                         for directories on all platforms (Windows, too).
+                         Exclusions are calculated first, inclusions later.
+                         [default: (\.smk$|^Snakefile)]
+
+  --exclude PATTERN      A regular expression that matches files and
+                         directories that should be excluded on recursive
+                         searches.  An empty value means no paths are
+                         excluded. Use forward slashes for directories on all
+                         platforms (Windows, too). Exclusions are calculated
+                         first, inclusions later.  [default: (\.snakemake|\.eg
+                         gs|\.git|\.hg|\.mypy_cache|\.nox|\.tox|\.venv|\.svn|_
+                         build|buck-out|build|dist)]
+
+  -c, --config PATH      Read configuration from PATH. By default, will try to
+                         read from `./pyproject.toml`
+
+  -h, --help             Show this message and exit.
+  -V, --version          Show the version and exit.
+  -v, --verbose          Turns on debug-level logging.
+
+```
+
+## Configuration
+
+`snakefmt` is able to read project-specific default values for its command line options
+from a `pyproject.toml` file. In addition, it will also load any [`black`
+configurations][black-config] you have in the same file.
+
+By default, `snakefmt` will search in the parent directories of the formatted file(s)
+for a file called `pyproject.toml` and use any configuration there.
+If your configuration file is located somewhere else or called something different,
+specify it using `--config`.
+
+Any options you pass on the command line will take precedence over default values in the
+configuration file.
+
+#### Example
+
+`pyproject.toml`
+
+```toml
+[tool.snakefmt]
+line_length = 90
+include = '\.smk$|^Snakefile|\.py$'
+
+# snakefmt passes these options on to black
+[tool.black]
+skip_string_normalization = true
+```
+
+In this example we increase the `--line-length` value and also include python (`*.py`)
+files for formatting - this effectively runs `black` on them. `snakefmt` will also pass
+on the `[tool.black]` settings, internally, to `black`.
+
+
+## Integration
+
+
+### Editor Integration
+
+For instructions on how to integrate `snakefmt` into your editor of choice, refer to
+[`docs/editor_integration.md`](docs/editor_integration.md)
+
+### Version Control Integration
+
+`snakefmt` supports [pre-commit](https://pre-commit.com/), a framework for managing git pre-commit hooks. Using this framework you can run `snakefmt` whenever you commit a `Snakefile` or `*.smk` file. `Pre-commit` automatically creates an isolated virtual environment with `snakefmt` and will stop the commit if `snakefmt` would modify the file. You then review, stage, and re-commit these changes. Pre-commit is especially useful if you don't have access to a CI/CD system like GitHub actions.
+
+To do so, create the file `.pre-commit-config.yaml` in the root of your project directory with the following:
+
+```yaml
+repos:
+  - repo: https://github.com/snakemake/snakefmt
+    rev: 0.5.0 # Replace by any tag/version ≥0.2.4 : https://github.com/snakemake/snakefmt/releases
+    hooks:
+      - id: snakefmt
+```
+
+Then [install pre-commit](https://pre-commit.com/#installation) and initialize the pre-commit hooks by running `pre-commit install` (Note you need to run this step once per clone of your repository). Additional pre-commit hooks can be found [here](https://pre-commit.com/hooks.html).
+
+### GitHub Actions
+
+[GitHub Actions](https://github.com/features/actions) in combination with [super-linter](https://github.com/github/super-linter) allows you to automatically run `snakefmt` on all Snakefiles in your repository e.g. whenever you push a new commit.
+
+To do so, create the file `.github/workflows/linter.yml` in your repository:
+```yaml
+---
+name: Lint Code Base
+
+on:
+  push:
+  pull_request:
+    branches: [master]
+
+jobs:
+  build:
+    name: Lint Code Base
+    runs-on: ubuntu-latest
+
+    steps:
+      - name: Checkout Code
+        uses: actions/checkout@v2
+
+      - name: Lint Code Base
+        uses: github/super-linter@v3
+        env:
+          VALIDATE_ALL_CODEBASE: false
+          DEFAULT_BRANCH: master
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+
+          VALIDATE_SNAKEMAKE_SNAKEFMT: true
+```
+
+Additional configuration parameters can be specified by creating `.github/linters/.snakefmt.toml`:
+```toml
+[tool.black]
+skip_string_normalization = true
+```
+
+For more information check the `super-linter` readme.
+
+## Plug Us
+
+If you can't get enough of badges, then feel free to show others you're using `snakefmt`
+in your project.
+
+[![Code style: snakefmt](https://img.shields.io/badge/code%20style-snakefmt-000000.svg)](https://github.com/snakemake/snakefmt)
+
+#### Markdown
+
+```md
+[![Code style: snakefmt](https://img.shields.io/badge/code%20style-snakefmt-000000.svg)](https://github.com/snakemake/snakefmt)
+```
+
+#### ReStructuredText
+
+```rst
+.. image:: https://img.shields.io/badge/code%20style-snakefmt-000000.svg
+    :target: https://github.com/snakemake/snakefmt
+```
+
+## Changes
+
+See [`CHANGELOG.md`][changes].
+
+## Contributing
+
+See [CONTRIBUTING.md][contributing].
+
+## Cite
+
+[![DOI][doi-shield]][doi]
+
+```Bibtex
+@article{snakemake2021,
+  doi = {10.12688/f1000research.29032.2},
+  url = {https://doi.org/10.12688/f1000research.29032.2},
+  year = {2021},
+  month = apr,
+  publisher = {F1000 Research Ltd},
+  volume = {10},
+  pages = {33},
+  author = {Felix M\"{o}lder and Kim Philipp Jablonski and Brice Letcher and Michael B. Hall and Christopher H. Tomkins-Tinch and Vanessa Sochat and Jan Forster and Soohyun Lee and Sven O. Twardziok and Alexander Kanitz and Andreas Wilm and Manuel Holtgrewe and Sven Rahmann and Sven Nahnsen and Johannes K\"{o}ster},
+  title = {Sustainable data analysis with Snakemake},
+  journal = {F1000Research}
 }
+```
+
 
+[snakemake]: https://snakemake.readthedocs.io/
+[black]: https://black.readthedocs.io/en/stable/
+[black-config]: https://github.com/psf/black#pyprojecttoml
+[pyproject]: https://github.com/snakemake/snakefmt/blob/master/pyproject.toml
+[poetry]: https://python-poetry.org
+[contributing]: CONTRIBUTING.md
+[changes]: CHANGELOG.md
+[doi-shield]: https://img.shields.io/badge/DOI-10.12688%2Ff1000research.29032.2-brightgreen.svg
+[doi]: https://doi.org/10.12688/f1000research.29032.2
 
-setup(**setup_kwargs)
```

