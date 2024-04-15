# Comparing `tmp/mdformat_admon-2.0.2.tar.gz` & `tmp/mdformat_admon-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdformat_admon-2.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mdformat_admon-2.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mdformat_admon-2.0.2.tar` & `mdformat_admon-2.0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1819 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/.gitignore
--rw-r--r--   0        0        0     1445 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      295 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/.pre-commit-test.yaml
--rw-r--r--   0        0        0     2853 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/.ruff.toml
--rw-r--r--   0        0        0       21 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/.tool-versions
--rw-r--r--   0        0        0     1365 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1073 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/LICENSE
--rw-r--r--   0        0        0     4140 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/README.md
--rw-r--r--   0        0        0      109 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/mdformat_admon/__init__.py
--rw-r--r--   0        0        0      176 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/mdformat_admon/factories/__init__.py
--rw-r--r--   0        0        0     6641 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/mdformat_admon/factories/_whitespace_admon_factories.py
--rw-r--r--   0        0        0      115 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/mdformat_admon/mdit_plugins/__init__.py
--rw-r--r--   0        0        0     2444 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/mdformat_admon/mdit_plugins/_python_markdown_admon.py
--rw-r--r--   0        0        0     1696 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/mdformat_admon/plugin.py
--rw-r--r--   0        0        0        0 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/mdformat_admon/py.typed
--rw-r--r--   0        0        0     1088 2024-03-12 00:28:04.734682 mdformat_admon-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      668 2024-03-12 00:28:04.738682 mdformat_admon-2.0.2/tox.ini
--rw-r--r--   0        0        0     4941 1970-01-01 00:00:00.000000 mdformat_admon-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      597 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/.copier-answers.yml
+-rw-r--r--   0        0        0     1819 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1592 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      295 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/.pre-commit-test.yaml
+-rw-r--r--   0        0        0     2881 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/.ruff.toml
+-rw-r--r--   0        0        0       21 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/.tool-versions
+-rw-r--r--   0        0        0      276 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/.yamllint.yaml
+-rw-r--r--   0        0        0     1365 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/LICENSE
+-rw-r--r--   0        0        0     4140 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/README.md
+-rw-r--r--   0        0        0      109 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/mdformat_admon/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/mdformat_admon/factories/__init__.py
+-rw-r--r--   0        0        0     6784 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/mdformat_admon/factories/_whitespace_admon_factories.py
+-rw-r--r--   0        0        0      115 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/mdformat_admon/mdit_plugins/__init__.py
+-rw-r--r--   0        0        0     2444 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/mdformat_admon/mdit_plugins/_python_markdown_admon.py
+-rw-r--r--   0        0        0     1766 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/mdformat_admon/plugin.py
+-rw-r--r--   0        0        0        0 2024-04-15 01:23:54.236498 mdformat_admon-2.0.3/mdformat_admon/py.typed
+-rw-r--r--   0        0        0     1180 2024-04-15 01:23:54.240498 mdformat_admon-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      753 2024-04-15 01:23:54.240498 mdformat_admon-2.0.3/tox.ini
+-rw-r--r--   0        0        0     4998 1970-01-01 00:00:00.000000 mdformat_admon-2.0.3/PKG-INFO
```

### Comparing `mdformat_admon-2.0.2/.gitignore` & `mdformat_admon-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mdformat_admon-2.0.2/.pre-commit-config.yaml` & `mdformat_admon-2.0.3/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,15 @@
       - id: check-vcs-permalinks
       - id: check-yaml
         args: [--unsafe]
       - id: debug-statements
       - id: destroyed-symlinks
       - id: detect-private-key
       - id: end-of-file-fixer
+        exclude: \.copier-answers\.yml
       - id: fix-byte-order-marker
       - id: fix-encoding-pragma
         args: [--remove]
       - id: forbid-new-submodules
       - id: mixed-line-ending
         args: [--fix=auto]
       - id: pretty-format-json
@@ -27,25 +28,29 @@
       - id: trailing-whitespace
         exclude: tests/.*fixtures.*\.md
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.13
+    rev: v0.3.4
     hooks:
       - id: ruff
         args: [--fix]
       - id: ruff-format
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
       - id: mdformat
-        additional_dependencies: ['mdformat-mkdocs[recommended]>=1.0.6']
+        additional_dependencies:
+          - mdformat-mkdocs[recommended]>=2.0.6
+          - mdformat-gfm-alerts>=0.0.1
         exclude: tests/.+\.md
         args: [--wrap=no]
-  - repo: https://github.com/lyz-code/yamlfix/
-    rev: 1.16.0
+  - repo: https://github.com/adrienverge/yamllint.git
+    rev: v1.35.1
     hooks:
-      - id: yamlfix
-        types_or: []
-        types: [file, yaml]
+      - id: yamllint
+  - repo: https://github.com/pappasam/toml-sort
+    rev: v0.23.1
+    hooks:
+      - id: toml-sort-fix
```

### Comparing `mdformat_admon-2.0.2/.ruff.toml` & `mdformat_admon-2.0.3/.ruff.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Docs: https://github.com/charliermarsh/ruff
 # Tip: run python -m ruff --explain RUF100
 
+line-length = 88
+target-version = 'py38'
+
+[lint]
 ignore = [
   'ANN002', # Missing type annotation for `*args`
   'ANN003', # Missing type annotation for `**kwargs`
   'ANN101', # Missing type annotation for `self` in method
   'ANN102', # Missing type annotation for `cls` in classmethod
   'ANN401', # Dynamically typed expressions (typing.Any) are disallowed in `**kwargs`
   'BLE001', # Do not catch blind exception: `Exception`
@@ -27,29 +31,27 @@
   'TCH003', # Move standard library import `pathlib.Path` into a type-checking block
   'TD001', # Invalid TODO tag: `FIXME`
   'TD002', # Missing author in TODO; try: `# TODO(<author_name>): ...`
   'TD003', # Missing issue link on the line following this TODO
   'TID252', # Relative imports from parent modules are banned
   'TRY003', # Avoid specifying long messages outside the exception class
 ]
-line-length = 88
 preview = true
 select = ['ALL']
-target-version = 'py38'
 unfixable = [
   'ERA001', # Commented out code
 ]
 
-[flake8-quotes]
+[lint.flake8-quotes]
 inline-quotes = 'double'
 
-[isort]
+[lint.isort]
 known-first-party = ['mdformat_admon']
 
-[per-file-ignores]
+[lint.per-file-ignores]
 '__init__.py' = [
   'D104', # Missing docstring in public package
   'F401', # imported but unused; consider adding to __all__ or using a redundant alias
 ]
 'tests/*.py' = [
   'ANN001', # Missing type annotation for function argument
   'ANN201', # Missing return type annotation for public function
@@ -59,9 +61,9 @@
   'D103', # Missing docstring in public function
   'EM102', # Exception must not use an f-string literal, assign to variable first
   'PT004', # flake8-pytest-style: fixture does not return
   'S101', # Use of `assert` detected
   'T201', # `print` found'
 ]
 
-[pylint]
+[lint.pylint]
 max-args = 6
```

### Comparing `mdformat_admon-2.0.2/CONTRIBUTING.md` & `mdformat_admon-2.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mdformat_admon-2.0.2/LICENSE` & `mdformat_admon-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mdformat_admon-2.0.2/README.md` & `mdformat_admon-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mdformat_admon-2.0.2/mdformat_admon/factories/_whitespace_admon_factories.py` & `mdformat_admon-2.0.3/mdformat_admon/factories/_whitespace_admon_factories.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Note, this is ported from `markdown-it-admon` <https://github.com/commenthol/markdown-it-admon>."""
 
 from __future__ import annotations
 
 import re
 from collections.abc import Generator, Sequence
 from contextlib import contextmanager, suppress
-from typing import TYPE_CHECKING, Callable, NamedTuple
+from typing import Callable, NamedTuple
 
 from markdown_it import MarkdownIt
+from markdown_it.renderer import RendererProtocol
+from markdown_it.ruler import RuleOptionsType
 from markdown_it.rules_block import StateBlock
+from markdown_it.token import Token
+from markdown_it.utils import EnvType, OptionsDict
 from mdit_py_plugins.utils import is_code_block
 
-if TYPE_CHECKING:
-    from markdown_it.renderer import RendererProtocol
-    from markdown_it.ruler import RuleOptionsType
-    from markdown_it.token import Token
-    from markdown_it.utils import EnvType, OptionsDict
-
 
 def _get_multiple_tags(meta_text: str) -> tuple[list[str], str]:
     """Check for multiple tags when the title is double quoted."""
     re_tags = re.compile(r'^\s*(?P<tokens>[^"]+)\s+"(?P<title>.*)"\S*$')
     if match := re_tags.match(meta_text):
         tags = match["tokens"].strip().split(" ")
         return [tag.lower() for tag in tags], match["title"]
@@ -71,29 +69,34 @@
 
 
 def search_admon_end(state: StateBlock, start_line: int, end_line: int) -> int:
     was_empty = False
 
     # Search for the end of the block
     next_line = start_line
+    is_fenced = False
     while True:
         next_line += 1
         if next_line >= end_line:
             # unclosed block should be autoclosed by end of document.
             # also block seems to be autoclosed by end of parent
             break
         pos = state.bMarks[next_line] + state.tShift[next_line]
         maximum = state.eMarks[next_line]
         is_empty = state.sCount[next_line] < state.blkIndent
 
-        # two consecutive empty lines autoclose the block
-        if is_empty and was_empty:
+        # two consecutive empty lines autoclose the block, unless the block is fenced
+        if not is_fenced and is_empty and was_empty:
             break
         was_empty = is_empty
 
+        # Check if line starts with ```
+        if state.src[pos : pos + 3] == "```":
+            is_fenced = not is_fenced
+
         if pos < maximum and state.sCount[next_line] < state.blkIndent:
             # non-empty line with negative indent should stop the block:
             # - !!!
             #  test
             break
 
     return next_line
```

### Comparing `mdformat_admon-2.0.2/mdformat_admon/mdit_plugins/_python_markdown_admon.py` & `mdformat_admon-2.0.3/mdformat_admon/mdit_plugins/_python_markdown_admon.py`

 * *Files identical despite different names*

### Comparing `mdformat_admon-2.0.2/mdformat_admon/plugin.py` & `mdformat_admon-2.0.3/mdformat_admon/plugin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """Auto-loaded plugin for mdformat."""
 
 from __future__ import annotations
 
 import textwrap
-from collections.abc import Mapping
 
 from markdown_it import MarkdownIt
 from mdformat.renderer import RenderContext, RenderTreeNode
 from mdformat.renderer.typing import Render
 
 from .mdit_plugins import python_markdown_admon_plugin
 
+try:
+    from beartype.typing import Mapping
+except ImportError:
+    from collections.abc import Mapping
+
 
 def update_mdit(mdit: MarkdownIt) -> None:
     """Update the parser with supported formats."""
     mdit.use(python_markdown_admon_plugin)
 
 
 def render_admon(node: RenderTreeNode, context: RenderContext) -> str:
```

### Comparing `mdformat_admon-2.0.2/pyproject.toml` & `mdformat_admon-2.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 [build-system]
-requires = ["flit_core >=3.2.0,<4"]
 build-backend = "flit_core.buildapi"
+requires = ["flit_core >=3.2.0,<4"]
 
 [project]
-name = "mdformat_admon"
 authors = [
-    { name = "Kyle King", email = "dev.act.kyle@gmail.com" },
+  {email = "dev.act.kyle@gmail.com", name = "kyleking"},
 ]
-readme = "README.md"
 classifiers = [
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
-    "Topic :: Software Development :: Libraries :: Python Modules",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Programming Language :: Python :: 3",
+  "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-keywords = ["mdformat", "markdown", "markdown-it"]
-requires-python = ">=3.8.0"
 dependencies = [
-    "mdformat >= 0.7.16",
-    "mdit-py-plugins >= 0.4.0",
+  "mdformat >= 0.7.16",
+  "mdit-py-plugins >= 0.4.0",
 ]
-dynamic = ["version", "description"]
+dynamic = ["description", "version"]
+keywords = ["markdown", "markdown-it", "mdformat"]
+name = "mdformat_admon"
+readme = "README.md"
+requires-python = ">=3.8.0"
+
+[project.entry-points."mdformat.parser_extension"]
+admon = "mdformat_admon"
 
 [project.optional-dependencies]
+dev = ["pre-commit"]
 test = [
-    "pytest >= 7.4.4",
-    "pytest-cov >= 4.1.0",
+  "pytest >= 7.4.4",
+  "pytest-beartype >= 0.0.2",
+  "pytest-cov >= 4.1.0",
 ]
-dev = ["pre-commit"]
 
 [project.urls]
-Homepage = "https://github.com/KyleKing/mdformat-admon"
-
-[project.entry-points."mdformat.parser_extension"]
-admonition = "mdformat_admon"
+homepage = "https://github.com/kyleking/mdformat-admon"
 
 [tool.flit.sdist]
-include = []
 exclude = [".github/", "tests/"]
+include = []
 
 [tool.pytest-watcher]
+ignore_patterns = []
 now = true
+patterns = ["*.md", "*.py"]
 runner = "tox"
-runner_args = ["-e", "py38"]
-patterns = ["*.py", "*.md"]
-ignore_patterns = []
+runner_args = ["-e", "py38-beartype"]
+
+[tool.tomlsort]
+all = true
+in_place = true
+trailing_comma_inline_array = true
```

### Comparing `mdformat_admon-2.0.2/tox.ini` & `mdformat_admon-2.0.3/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [tox]
 envlist =
-    py{38}
+    py{38}-beartype
     py{312}-cov
     py{312}-pre-commit
     py{38}-hook
     mypy
     ruff
 isolated_build = True
 skip_missing_interpreters = False
 
-[testenv:py{38}]
+[testenv:py{38}-beartype]
 extras = test
-commands = pytest {posargs} --ff --nf -vv
+commands = pytest {posargs} --ff --nf -vv --exitfirst --beartype-packages='mdformat_admon'
 
 [testenv:py{312}-cov]
 extras = test
 commands = pytest --cov=mdformat_admon {posargs}
 
 [testenv:py{312}-pre-commit]
 extras = dev
 commands = pre-commit run {posargs:--all-files}
 
 [testenv:py{38}-hook]
 extras = dev
 commands = pre-commit run --config .pre-commit-test.yaml {posargs:--all-files --verbose --show-diff-on-failure}
 
 [testenv:mypy]
-deps = mypy
+deps =
+    beartype
+    mypy
 commands = mypy ./mdformat_admon
 
 [testenv:ruff]
 deps = ruff
-commands = ruff . --fix
+commands = ruff format .
```

### Comparing `mdformat_admon-2.0.2/PKG-INFO` & `mdformat_admon-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: mdformat_admon
-Version: 2.0.2
+Version: 2.0.3
 Summary: An mdformat plugin for admonitions.
-Keywords: mdformat,markdown,markdown-it
-Author-email: Kyle King <dev.act.kyle@gmail.com>
+Keywords: markdown,markdown-it,mdformat
+Author-email: kyleking <dev.act.kyle@gmail.com>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: mdformat >= 0.7.16
 Requires-Dist: mdit-py-plugins >= 0.4.0
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest >= 7.4.4 ; extra == "test"
+Requires-Dist: pytest-beartype >= 0.0.2 ; extra == "test"
 Requires-Dist: pytest-cov >= 4.1.0 ; extra == "test"
-Project-URL: Homepage, https://github.com/KyleKing/mdformat-admon
+Project-URL: homepage, https://github.com/kyleking/mdformat-admon
 Provides-Extra: dev
 Provides-Extra: test
 
 # mdformat-admon
 
 [![Build Status][ci-badge]][ci-link] [![PyPI version][pypi-badge]][pypi-link]
```

