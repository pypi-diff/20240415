# Comparing `tmp/pyreball-2.0.0.tar.gz` & `tmp/pyreball-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreball-2.0.0.tar", last modified: Wed Nov 15 19:25:20 2023, max compression
+gzip compressed data, was "pyreball-2.1.0.tar", max compression
```

## Comparing `pyreball-2.0.0.tar` & `pyreball-2.1.0.tar`

### file list

```diff
@@ -1,44 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:25:20.396849 pyreball-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-11-15 19:25:06.000000 pyreball-2.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2023-11-15 19:25:06.000000 pyreball-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-11-15 19:25:06.000000 pyreball-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-11-15 19:25:20.392849 pyreball-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2023-11-15 19:25:06.000000 pyreball-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:25:20.392849 pyreball-2.0.0/pyreball/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25080 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/_common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:25:20.392849 pyreball-2.0.0/pyreball/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/cfg/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/cfg/css.template
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/cfg/external_links.ini
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/cfg/html.template
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    42338 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/html.py
--rw-r--r--   0 runner    (1001) docker     (127)    16683 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:25:20.392849 pyreball-2.0.0/pyreball/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    13500 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/utils/param.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball/utils/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:25:20.392849 pyreball-2.0.0/pyreball.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-11-15 19:25:20.000000 pyreball-2.0.0/pyreball.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-11-15 19:25:20.000000 pyreball-2.0.0/pyreball.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 19:25:20.000000 pyreball-2.0.0/pyreball.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-15 19:25:20.000000 pyreball-2.0.0/pyreball.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-15 19:25:20.000000 pyreball-2.0.0/pyreball.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    71396 2023-11-15 19:25:06.000000 pyreball-2.0.0/pyreball_result_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-15 19:25:06.000000 pyreball-2.0.0/requirements_examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-15 19:25:06.000000 pyreball-2.0.0/requirements_examples_py38.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-11-15 19:25:06.000000 pyreball-2.0.0/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 19:25:20.396849 pyreball-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2023-11-15 19:25:06.000000 pyreball-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:25:20.392849 pyreball-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    62059 2023-11-15 19:25:06.000000 pyreball-2.0.0/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (127)    24268 2023-11-15 19:25:06.000000 pyreball-2.0.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2023-11-15 19:25:06.000000 pyreball-2.0.0/tests/test_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:25:20.392849 pyreball-2.0.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 19:25:06.000000 pyreball-2.0.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19388 2023-11-15 19:25:06.000000 pyreball-2.0.0/tests/utils/test_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2023-11-15 19:25:06.000000 pyreball-2.0.0/tests/utils/test_template.py
+-rw-r--r--   0        0        0    11344 2024-04-15 19:48:17.769266 pyreball-2.1.0/LICENSE
+-rw-r--r--   0        0        0     4128 2024-04-15 19:48:17.769266 pyreball-2.1.0/README.md
+-rw-r--r--   0        0        0     3254 2024-04-15 19:48:17.769266 pyreball-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      739 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/__init__.py
+-rw-r--r--   0        0        0    25870 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/__main__.py
+-rw-r--r--   0        0        0      597 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/_common.py
+-rw-r--r--   0        0        0      573 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/cfg/config.ini
+-rw-r--r--   0        0        0     1486 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/cfg/css.template
+-rw-r--r--   0        0        0     1594 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/cfg/external_links.ini
+-rw-r--r--   0        0        0      316 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/cfg/html.template
+-rw-r--r--   0        0        0     1534 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/config_generator.py
+-rw-r--r--   0        0        0      212 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/constants.py
+-rw-r--r--   0        0        0    42545 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/html.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/py.typed
+-rw-r--r--   0        0        0    16707 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/text.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/utils/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/utils/logger.py
+-rw-r--r--   0        0        0    13435 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/utils/param.py
+-rw-r--r--   0        0        0     1059 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/utils/template.py
+-rw-r--r--   0        0        0     6104 1970-01-01 00:00:00.000000 pyreball-2.1.0/PKG-INFO
```

### Comparing `pyreball-2.0.0/LICENSE` & `pyreball-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyreball-2.0.0/README.md` & `pyreball-2.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Pyreball
 
 <p style="text-align: center">
 
-![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)
+![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 [![pypi](https://img.shields.io/pypi/v/pyreball.svg)](https://pypi.python.org/pypi/pyreball)
-[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Tests](https://github.com/karelvaculik/pyreball/actions/workflows/tests.yml/badge.svg)](https://github.com/karelvaculik/pyreball/actions/workflows/tests.yml)
 
 </p>
 
 Pyreball is a Python reporting tool that generates HTML reports from Python scripts.
 
 Main features:
```

### Comparing `pyreball-2.0.0/pyreball/__init__.py` & `pyreball-2.1.0/src/pyreball/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-__version__ = "2.0.0"
-
 from pyreball.html import (
+    Reference,
     print,
     print_code_block,
     print_div,
     print_figure,
     print_h1,
     print_h2,
     print_h3,
     print_h4,
     print_h5,
     print_h6,
     print_table,
-    Reference,
     set_title,
 )
 from pyreball.text import (
     a,
     bold,
     code,
     code_block,
```

### Comparing `pyreball-2.0.0/pyreball/__main__.py` & `pyreball-2.1.0/src/pyreball/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 import argparse
 import json
 import os
 import re
 import sys
 import textwrap
+import typing
 import xml
 from pathlib import Path
-from typing import cast, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union, cast
 from xml.dom.minidom import parseString
 
-import pkg_resources
-
+from pyreball._common import get_default_path_to_config
 from pyreball.constants import (
     CONFIG_INI_FILENAME,
-    DEFAULT_PATH_TO_CONFIG,
     HTML_TEMPLATE_FILENAME,
     LINKS_INI_FILENAME,
     STYLES_TEMPLATE_FILENAME,
 )
 from pyreball.utils.logger import get_logger
 from pyreball.utils.param import (
+    ChoiceParameter,
+    IntegerParameter,
+    StringParameter,
+    Substitutor,
     carefully_remove_directory_if_exists,
     check_and_fix_parameters,
     check_paging_sizes_string_parameter,
-    ChoiceParameter,
     get_external_links_from_config,
     get_file_config,
-    IntegerParameter,
     merge_parameter_dictionaries,
-    StringParameter,
-    Substitutor,
 )
 from pyreball.utils.template import get_css, get_html
 
 logger = get_logger()
 
 
 def _replace_ids(lines: List[str]) -> List[str]:
@@ -196,15 +195,15 @@
             current_line = f'<a href="#{h[1]}">{h[2]}</a><br/>\n'
         else:
             current_line = f'<li><a href="#{h[1]}">{h[2]}</a></li>\n'
         lines.insert(lines_index, current_line)
         lines_index += 1
 
     # at the end, get back to level 1 if necessary
-    while 1 < current_level:
+    while current_level > 1:
         lines.insert(lines_index, "</ul>\n")
         lines_index += 1
         current_level -= 1
 
     return lines
 
 
@@ -228,17 +227,19 @@
 
 
 def _insert_js_and_css_links(
     html_content: str, external_links: Dict[str, List[str]]
 ) -> str:
     groups_of_links_to_add = set()
     add_jquery = False
-    if _contains_class(
-        html_text=html_content, class_name="inline-highlight"
-    ) or _contains_class(html_text=html_content, class_name="pyreball-code-wrapper"):
+    if (
+        _contains_class(html_text=html_content, class_name="inline-highlight")
+        or _contains_class(html_text=html_content, class_name="block-highlight")
+        or _contains_class(html_text=html_content, class_name="pyreball-code-wrapper")
+    ):
         add_jquery = True
         groups_of_links_to_add.add("highlight_js")
     if _contains_class(html_text=html_content, class_name="pyreball-table-wrapper"):
         add_jquery = True
         groups_of_links_to_add.add("datatables")
     if _contains_class(html_text=html_content, class_name="pyreball-altair-fig"):
         groups_of_links_to_add.add("altair")
@@ -248,15 +249,15 @@
         groups_of_links_to_add.add("bokeh")
 
     # gather all links; jquery must be first
     links_to_add = "\n".join(
         (external_links["jquery"] if add_jquery else [])
         + [
             el
-            for group in sorted(list(groups_of_links_to_add))
+            for group in sorted(groups_of_links_to_add)
             for el in external_links[group]
         ]
     )
     html_content = re.sub("<!--PYREBALL_HEAD_LINKS-->", links_to_add, html_content)
     return html_content
 
 
@@ -289,15 +290,15 @@
     """
     Load the printed HTML and finish substitutions to make it complete.
 
     Args:
         html_path: Path to the HTML file.
         include_toc: Whether to include the table of contents.
     """
-    with open(html_path, "r") as f:
+    with open(html_path) as f:
         lines = f.readlines()
 
     lines = _replace_ids(lines)
     lines = _insert_heading_title_and_toc(lines=lines, include_toc=include_toc)
 
     html_content = "".join(lines)
     html_content = _insert_js_and_css_links(html_content, external_links)
@@ -514,20 +515,20 @@
     if home_config_dir_path.exists():
         _check_existence_of_config_files(
             config_dir_path=home_config_dir_path, recommendation_msg=rec_msg
         )
         return home_config_dir_path
 
     # Fallback to the default config directory in installation directory
-    default_config_dir_path = DEFAULT_PATH_TO_CONFIG
+    default_config_dir_path = get_default_path_to_config()
     _check_existence_of_config_files(
         config_dir_path=default_config_dir_path,
         recommendation_msg="Try re-installing pyreball.",
     )
-    return default_config_dir_path
+    return default_config_dir_path  # type: ignore[no-any-return]
 
 
 def _get_output_dir_and_file_stem(
     input_path: Path, output_path_str: Optional[Path]
 ) -> Tuple[Path, str]:
     """
     Obtain the output directory for the HTML file and output filename stem.
@@ -561,26 +562,34 @@
             filename_stem = input_path.stem
         output_dir_path.mkdir(parents=True, exist_ok=True)
 
     return output_dir_path, filename_stem
 
 
 class PathAction(argparse.Action):
-    def __call__(self, parser, namespace, values, option_string=None):
+    def __call__(
+        self,
+        parser: argparse.ArgumentParser,
+        namespace: argparse.Namespace,
+        values: Optional[Union[str, Sequence[Any]]],
+        option_string: Optional[str] = None,
+    ) -> None:
         if values is None:
             setattr(namespace, self.dest, values)
-        else:
+        elif isinstance(values, str):
             if values.strip() == "":
                 raise argparse.ArgumentError(
                     self, "Path argument cannot contain only whitespaces."
                 )
             setattr(namespace, self.dest, Path(values))
+        else:
+            raise ValueError("Unexpected argument type for values.")
 
 
-def parse_arguments(args) -> Dict[str, Optional[Union[str, int]]]:
+def parse_arguments(args: List[str]) -> Dict[str, Optional[Union[str, int]]]:
     parser = argparse.ArgumentParser(
         description=(
             "Generate Python report. "
             "Any options or arguments after '--' are passed "
             "to the processed Python script / module. "
         )
     )
@@ -650,14 +659,30 @@
     return variables
 
 
 def _convert_module_to_path(mod: str) -> Path:
     return Path(mod.replace(".", os.sep) + ".py")
 
 
+@typing.no_type_check
+def _get_path_to_html_template() -> Path:
+    try:
+        # Python >=3.9
+        from importlib.resources import files  # type: ignore[attr-defined]
+
+        return Path(files("pyreball") / "cfg" / HTML_TEMPLATE_FILENAME)
+    except ImportError:
+        # Python 3.8
+        import pkg_resources
+
+        return Path(
+            pkg_resources.resource_filename("pyreball", f"cfg/{HTML_TEMPLATE_FILENAME}")
+        )
+
+
 def main() -> None:
     args_dict = parse_arguments(sys.argv[1:])
     script_args_string = " ".join(cast(List[str], args_dict.pop("script_args")))
     if args_dict["input_path"]:
         input_path = cast(Path, args_dict.pop("input_path"))
         input_path = input_path.expanduser().resolve()
         path_arg = str(input_path)
@@ -713,17 +738,15 @@
     css_definitions = get_css(
         filename=STYLES_TEMPLATE_FILENAME,
         directory=config_directory,
         page_width=cast(int, parameters["page_width"]),
     )
 
     html_begin, html_end = get_html(
-        template_path=Path(
-            pkg_resources.resource_filename("pyreball", f"cfg/{HTML_TEMPLATE_FILENAME}")
-        ),
+        template_path=_get_path_to_html_template(),
         title=filename_stem,
         css_definitions=css_definitions,
     )
 
     with open(html_path, "w") as f:
         f.write(html_begin)
     try:
```

### Comparing `pyreball-2.0.0/pyreball/cfg/config.ini` & `pyreball-2.1.0/src/pyreball/cfg/config.ini`

 * *Files identical despite different names*

### Comparing `pyreball-2.0.0/pyreball/cfg/css.template` & `pyreball-2.1.0/src/pyreball/cfg/css.template`

 * *Files identical despite different names*

### Comparing `pyreball-2.0.0/pyreball/cfg/external_links.ini` & `pyreball-2.1.0/src/pyreball/cfg/external_links.ini`

 * *Files 2% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 datatables =
     <link rel="stylesheet" href="https://cdn.datatables.net/1.13.6/css/jquery.dataTables.min.css" />
     <script src="https://cdn.datatables.net/1.13.6/js/jquery.dataTables.min.js"></script>
 highlight_js =
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/styles/default.min.css">
     <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/highlight.min.js"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/languages/python.min.js"></script>
-    <script>hljs.highlightAll();</script>
+    <script>hljs.configure({cssSelector: 'pre code.block-highlight'});hljs.highlightAll();</script>
 jquery =
     <script src="https://code.jquery.com/jquery-3.7.0.js"></script>
 plotly =
     <script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
```

### Comparing `pyreball-2.0.0/pyreball/html.py` & `pyreball-2.1.0/src/pyreball/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,69 +1,68 @@
 """Main functions that serve as building blocks of the final html file."""
+
 import builtins
 import io
 import json
 import os
 import random
 import re
 from typing import (
+    TYPE_CHECKING,
     Any,
-    cast,
     Dict,
     List,
-    Literal,
     Optional,
     Set,
     Tuple,
-    TYPE_CHECKING,
     Union,
+    cast,
 )
 
 from pyreball._common import AttrsParameter, ClParameter
 from pyreball.constants import NON_BREAKABLE_SPACE, PILCROW_SIGN
-
 from pyreball.text import code_block, div
 from pyreball.utils.param import get_parameter_value, make_sure_dir_exists, merge_values
 
 if TYPE_CHECKING:
     # needed for mypy
     # noinspection PyUnresolvedReferences,PyPackageRequirements
-    import altair  # type: ignore
+    import altair  # type: ignore[unused-ignore]
 
     # noinspection PyPackageRequirements
-    import bokeh  # type: ignore
+    import bokeh  # type: ignore[unused-ignore]
 
     # noinspection PyPackageRequirements
-    import matplotlib  # type: ignore
+    import matplotlib  # type: ignore[unused-ignore]
 
     # noinspection PyPackageRequirements
-    import pandas  # type: ignore
+    import pandas  # type: ignore[unused-ignore]
 
     # noinspection PyPackageRequirements
-    import plotly  # type: ignore
+    import plotly  # type: ignore[unused-ignore]
 
 AltairFigType = Union[
-    "altair.vegalite.v4.api.Chart",
-    "altair.vegalite.v4.api.ConcatChart",
-    "altair.vegalite.v4.api.FacetChart",
-    "altair.vegalite.v4.api.HConcatChart",
-    "altair.vegalite.v4.api.LayerChart",
-    "altair.vegalite.v4.api.RepeatChart",
-    "altair.vegalite.v4.api.VConcatChart",
+    "altair.vegalite.v5.api.Chart",
+    "altair.vegalite.v5.api.ConcatChart",
+    "altair.vegalite.v5.api.FacetChart",
+    "altair.vegalite.v5.api.HConcatChart",
+    "altair.vegalite.v5.api.LayerChart",
+    "altair.vegalite.v5.api.RepeatChart",
+    "altair.vegalite.v5.api.VConcatChart",
 ]
 FigType = Union[
     "matplotlib.figure.Figure",
     "plotly.graph_objs._figure.Figure",
-    "altair.vegalite.v4.api.Chart",
-    "altair.vegalite.v4.api.ConcatChart",
-    "altair.vegalite.v4.api.FacetChart",
-    "altair.vegalite.v4.api.HConcatChart",
-    "altair.vegalite.v4.api.LayerChart",
-    "altair.vegalite.v4.api.RepeatChart",
-    "altair.vegalite.v4.api.VConcatChart",
+    "altair.vegalite.v5.api.Chart",
+    "altair.vegalite.v5.api.ConcatChart",
+    "altair.vegalite.v5.api.FacetChart",
+    "altair.vegalite.v5.api.HConcatChart",
+    "altair.vegalite.v5.api.LayerChart",
+    "altair.vegalite.v5.api.RepeatChart",
+    "altair.vegalite.v5.api.VConcatChart",
 ]
 
 _references: Set[str] = set()
 _heading_memory: Dict[str, Any] = {}
 _code_block_memory: Dict[str, Any] = {}
 _table_memory: Dict[str, Any] = {}
 _graph_memory: Dict[str, Any] = {}
@@ -148,15 +147,15 @@
         title: Title string.
     """
     if not get_parameter_value("html_file_path") or get_parameter_value("keep_stdout"):
         builtins.print(title)
     if get_parameter_value("html_file_path"):
         # it is assumed that the heading is already written into the file,
         # so find the line with title element and replace its contents
-        with open(get_parameter_value("html_file_path"), "r") as f:
+        with open(get_parameter_value("html_file_path")) as f:
             lines = f.readlines()
 
         # replace the title and also add "custom_pyreball_title" class,
         # so that we know it was replaced by this function
         lines = [
             re.sub(
                 r"^<title>[^<]*</title>",
@@ -371,15 +370,15 @@
     code_block_index: int = 0,
     caption: Optional[str] = None,
     reference: Optional[Reference] = None,
     align: str = "center",
     caption_position: str = "bottom",
     numbered: bool = True,
     sep: str = "",
-):
+) -> str:
     if reference:
         _check_and_mark_reference(reference)
         anchor_link = f"code-block-{reference.id}-{code_block_index}"
     else:
         anchor_link = f"code-block-{code_block_index}"
 
     caption_element = _prepare_caption_element(
@@ -422,15 +421,15 @@
     numbered: Optional[bool] = None,
     cl: ClParameter = None,
     attrs: AttrsParameter = None,
     pre_cl: ClParameter = None,
     pre_attrs: AttrsParameter = None,
     sep: str = "",
     end: str = "\n",
-    syntax_highlight: Optional[Literal["python"]] = "python",
+    syntax_highlight: Optional[str] = "python",
 ) -> None:
     """
     Print values as a source code into a preformatted block.
 
     This element is used to display a source code in a block.
     It is possible to highlight the code syntax by setting `syntax_highlight`
     parameter to an appropriate string.
@@ -459,17 +458,20 @@
             To construct boolean HTML attributes, set `None` for given key.
             Any quotes in values are not escaped.
         pre_cl: The same as `cl` parameter, but for the `<pre>` tag.
         pre_attrs: The same as `attrs` parameter, but for the `<pre>` tag.
         sep: String separator of the values inside the tag. Defaults to an empty string.
         end: String appended after the tag. Defaults to a newline.
         syntax_highlight: Syntax highlighting language.
-            Currently only `'python'` is supported. If `None`,
-            no highlight is applied. When highlight is turned on,
-            language name is added to the `<code>` element as a class.
+            Supported values can be obtained from highlight.js table
+            https://github.com/highlightjs/highlight.js/blob/main/SUPPORTED_LANGUAGES.md
+            - see column "Aliases". If `None`, no highlighting is applied.
+            When highlight is turned on, language name and `'block-highlight'`
+            are added to the `<code>` element as classes.
+
     """
 
     source_code_str = code_block(
         *values,
         cl=cl,
         attrs=attrs,
         pre_cl=pre_cl,
@@ -539,31 +541,28 @@
 
 
 def _prepare_caption_element(
     prefix: str, caption: Optional[str], numbered: bool, index: int, anchor_link: str
 ) -> str:
     if numbered:
         caption_text = f"{prefix} {index}"
-        if caption:
-            caption_text = f"{caption_text}: {caption}"
-        else:
-            caption_text = f"{caption_text}."
+        caption_text = f"{caption_text}: {caption}" if caption else f"{caption_text}."
     elif caption:
         caption_text = f"{caption}"
     else:
         caption_text = ""
     return (
         f'\n<div class="pyreball-text-centered">'
         f'<a id="{anchor_link}"><b>\n{caption_text}\n</b></a>'
         f"</div>\n"
     )
 
 
 def _compute_length_menu_for_datatables(
-    paging_sizes: List[Union[int, str]]
+    paging_sizes: List[Union[int, str]],
 ) -> Tuple[List[int], List[Union[int, str]]]:
     arr_1: List[int] = []
     arr_2: List[Union[int, str]] = []
     for size in paging_sizes:
         if isinstance(size, int):
             arr_1.append(size)
             arr_2.append(size)
@@ -620,15 +619,15 @@
 
     if col_align_def is not None:
         datatables_setup["columnDefs"] = col_align_def
 
     return datatables_setup
 
 
-def _check_col_alignment_value(value: str):
+def _check_col_alignment_value(value: str) -> None:
     allowed_values = ["left", "center", "right"]
     if value not in allowed_values:
         raise ValueError(
             "col_align must use only the following values: "
             f"{', '.join(allowed_values)}."
         )
 
@@ -1024,20 +1023,20 @@
     img_element += 'var opt = {"renderer": "canvas", "actions": false};\n'
     img_element += f'vegaEmbed("#{vis_id}", spec, opt);'
     img_element += "</script>"
     return img_element
 
 
 def _prepare_plotly_image_element(fig: "plotly.graph_objs.Figure") -> str:
-    return fig.to_html(full_html=False, include_plotlyjs=False)
+    return cast(str, fig.to_html(full_html=False, include_plotlyjs=False))
 
 
 def _prepare_bokeh_image_element(fig: "bokeh.plotting._figure.figure") -> str:
     # noinspection PyPackageRequirements
-    from bokeh.embed import components  # type: ignore
+    from bokeh.embed import components  # type: ignore[unused-ignore]
 
     script, div = components(fig)
     return f"<div>{div}{script}</div>"
 
 
 def _prepare_image_element(
     fig: FigType,
```

### Comparing `pyreball-2.0.0/pyreball/text.py` & `pyreball-2.1.0/src/pyreball/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Text utils for creating strings with HTML elements."""
-from typing import Any, List, Literal, Optional
+
+from typing import Any, List, Optional
 
 from pyreball._common import AttrsParameter, ClParameter
 
 
 def _construct_attrs_str(attrs: AttrsParameter) -> Optional[str]:
     if not attrs:
         return None
@@ -11,18 +12,15 @@
         [f'{k}="{v}"' if v is not None else f"{k}" for k, v in attrs.items()]
     )
 
 
 def _construct_class_attr_string(cl: ClParameter) -> Optional[str]:
     if cl is None:
         return None
-    if isinstance(cl, str):
-        cl_values = cl
-    else:
-        cl_values = " ".join(cl)
+    cl_values = cl if isinstance(cl, str) else " ".join(cl)
     return _construct_attrs_str({"class": cl_values})
 
 
 def bold(
     *values: Any, cl: ClParameter = None, attrs: AttrsParameter = None, sep: str = ""
 ) -> str:
     """
@@ -75,39 +73,34 @@
     """
     return tag(*values, name="em", cl=cl, attrs=attrs, sep=sep)
 
 
 def _collect_classes_for_code_strings(
     initial_class_list: List[str],
     cl: ClParameter,
-    syntax_highlight: Optional[Literal["python"]],
+    syntax_highlight: Optional[str],
 ) -> ClParameter:
     classes_to_be_added = initial_class_list[:]
     if syntax_highlight is not None:
-        if syntax_highlight == "python":
-            classes_to_be_added.append("python")
-        else:
-            raise ValueError(
-                f"Unsupported syntax highlighting language: {syntax_highlight}."
-            )
+        classes_to_be_added.append(syntax_highlight)
         if cl is None:
             cl = classes_to_be_added
         elif isinstance(cl, str):
-            cl = [cl] + classes_to_be_added
+            cl = [cl, *classes_to_be_added]
         else:
             cl = cl + classes_to_be_added
     return cl
 
 
 def code(
     *values: Any,
     cl: ClParameter = None,
     attrs: AttrsParameter = None,
     sep: str = "",
-    syntax_highlight: Optional[Literal["python"]] = "python",
+    syntax_highlight: Optional[str] = "python",
 ) -> str:
     """
     Create a `<code>` element string with given values.
 
     This element is used to display a source code inline.
     It is possible to highlight the code syntax by setting `syntax_highlight`
     parameter to an appropriate string.
@@ -123,15 +116,17 @@
         attrs: Additional attributes to be added to the tag.
             Dictionary `{"key1": "value1", ..., "keyN": "valueN"}`
             is converted to `key1="value1" ... keyN="valueN"`.
             To construct boolean HTML attributes,
             set `None` for given key. Any quotes in values are not escaped.
         sep: String separator of the values. Defaults to an empty string.
         syntax_highlight: Syntax highlighting language.
-            Currently only `'python'` is supported. If `None`, no highlight is applied.
+            Supported values can be obtained from highlight.js table
+            https://github.com/highlightjs/highlight.js/blob/main/SUPPORTED_LANGUAGES.md
+            - see column "Aliases". If `None`, no highlighting is applied.
             When highlight is turned on, language name and `'inline-highlight'`
             are added to the element as classes.
 
     Returns:
         HTML string representing the tag with given values.
     """
     cl = _collect_classes_for_code_strings(["inline-highlight"], cl, syntax_highlight)
@@ -141,15 +136,15 @@
 def code_block(
     *values: Any,
     cl: ClParameter = None,
     attrs: AttrsParameter = None,
     pre_cl: ClParameter = None,
     pre_attrs: AttrsParameter = None,
     sep: str = "",
-    syntax_highlight: Optional[Literal["python"]] = "python",
+    syntax_highlight: Optional[str] = "python",
 ) -> str:
     """
     Create a `<pre><code>` pair element string with given values.
 
     This element is used to display a source code in a block.
     It is possible to highlight the code syntax by setting `syntax_highlight`
     parameter to an appropriate string.
@@ -168,22 +163,24 @@
             is converted to `key1="value1" ... keyN="valueN"`.
             To construct boolean HTML attributes,
             set `None` for given key. Any quotes in values are not escaped.
         pre_cl: The same as `cl` parameter, but for the `<pre>` tag.
         pre_attrs: The same as `attrs` parameter, but for the `<pre>` tag.
         sep: String separator of the values. Defaults to an empty string.
         syntax_highlight: Syntax highlighting language.
-            Currently only `'python'` is supported. If `None`, no highlight is applied.
-            When highlight is turned on, language name is added to the `<code>`
-            element as a class.
+            Supported values can be obtained from highlight.js table
+            https://github.com/highlightjs/highlight.js/blob/main/SUPPORTED_LANGUAGES.md
+            - see column "Aliases". If `None`, no highlighting is applied.
+            When highlight is turned on, language name and `'block-highlight'`
+            are added to the element as classes.
 
     Returns:
         HTML string representing the tag with given values.
     """
-    cl = _collect_classes_for_code_strings([], cl, syntax_highlight)
+    cl = _collect_classes_for_code_strings(["block-highlight"], cl, syntax_highlight)
     code_text = tag(*values, name="code", cl=cl, attrs=attrs, sep=sep)
     return tag(code_text, name="pre", cl=pre_cl, attrs=pre_attrs)
 
 
 def div(
     *values: Any, cl: ClParameter = None, attrs: AttrsParameter = None, sep: str = ""
 ) -> str:
@@ -281,21 +278,18 @@
 
 
 def _enclose_into_li_tags(
     *values: Any,
     cl: ClParameter = None,
     attrs: AttrsParameter = None,
     sep: str = "",
-):
+) -> str:
     result = ""
     for value in values:
-        if isinstance(value, tuple):
-            value_str = "".join(map(str, value))
-        else:
-            value_str = str(value)
+        value_str = "".join(map(str, value)) if isinstance(value, tuple) else str(value)
         result += tag(value_str, name="li", cl=cl, attrs=attrs, sep=sep)
     return result
 
 
 def ulist(
     *values: Any,
     cl: ClParameter = None,
```

### Comparing `pyreball-2.0.0/pyreball/utils/param.py` & `pyreball-2.1.0/src/pyreball/utils/param.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import os
 import re
 import shutil
 import sys
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
 
 from pyreball.utils.logger import get_logger
 
 ParametersType = Dict[str, Optional[Union[str, int]]]
 
 logger = get_logger()
 
@@ -23,49 +23,45 @@
         self.option_string = option_string
         self._config_param_key = option_string.replace("--", "")
         self._param_key = self._config_param_key.replace("-", "_")
         self.help = help
 
     @property
     @abstractmethod
-    def param_key(self):
-        ...
+    def param_key(self) -> str: ...
 
     @property
     @abstractmethod
-    def config_param_key(self):
-        ...
+    def config_param_key(self) -> str: ...
 
     @abstractmethod
-    def add_argument_to_parser(self, parser: argparse.ArgumentParser) -> None:
-        ...
+    def add_argument_to_parser(self, parser: argparse.ArgumentParser) -> None: ...
 
     @abstractmethod
     def check_and_fix_value(
         self,
         value: Any,
         none_allowed: bool,
         warning_messages: List[str],
         error_messages: List[str],
-    ) -> Any:
-        ...
+    ) -> Any: ...
 
 
 class ChoiceParameter(Parameter):
     def __init__(self, option_string: str, choices: List[str], default: str, help: str):
         super().__init__(option_string=option_string, help=help)
         self.default = default
         self.choices = choices
 
     @property
-    def param_key(self):
+    def param_key(self) -> str:
         return self._param_key
 
     @property
-    def config_param_key(self):
+    def config_param_key(self) -> str:
         return self._config_param_key
 
     def add_argument_to_parser(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(self.option_string, choices=self.choices, help=self.help)
 
     def check_and_fix_value(
         self,
@@ -94,19 +90,19 @@
         help: str,
     ):
         super().__init__(option_string=option_string, help=help)
         self.boundaries = boundaries
         self.default = default
 
     @property
-    def param_key(self):
+    def param_key(self) -> str:
         return self._param_key
 
     @property
-    def config_param_key(self):
+    def config_param_key(self) -> str:
         return self._config_param_key
 
     def add_argument_to_parser(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(self.option_string, type=int, help=self.help)
 
     def check_and_fix_value(
         self,
@@ -139,19 +135,19 @@
         ] = None,
     ):
         super().__init__(option_string=option_string, help=help)
         self.default = default
         self.validation_function = validation_function
 
     @property
-    def param_key(self):
+    def param_key(self) -> str:
         return self._param_key
 
     @property
-    def config_param_key(self):
+    def config_param_key(self) -> str:
         return self._config_param_key
 
     def add_argument_to_parser(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(self.option_string, type=str, help=self.help)
 
     def check_and_fix_value(
         self,
@@ -347,15 +343,15 @@
         "highlight_js",
         "jquery",
         "plotly",
     }
     if links.keys() != required_keys:
         logger.error(
             "Configuration with items must contain links for exactly these keys: "
-            f"{', '.join(sorted(list(required_keys)))}."
+            f"{', '.join(sorted(required_keys))}."
         )
         sys.exit(1)
     return links
 
 
 def merge_values(primary_value: Any, secondary_value: Any) -> Any:
     return primary_value if primary_value is not None else secondary_value
@@ -371,23 +367,16 @@
             primary_value=primary_parameters.get(param_spec.param_key),
             secondary_value=secondary_parameters.get(param_spec.param_key),
         )
         for param_spec in parameter_specifications
     }
 
 
-def _map_env_value(value):
-    if value == "None":
-        return None
-    elif value == "yes":
-        return True
-    elif value == "no":
-        return False
-    else:
-        return value
+def _map_env_value(value: str) -> Any:
+    return {"None": None, "yes": True, "no": False}.get(value, value)
 
 
 def get_parameter_value(key: str) -> Any:
     if "params" not in _parameter_cache:
         _parameter_cache["params"] = {
             k: _map_env_value(v)
             for k, v in json.loads(
```

### Comparing `pyreball-2.0.0/pyreball/utils/template.py` & `pyreball-2.1.0/src/pyreball/utils/template.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pyreball.utils.logger import get_logger
 
 logger = get_logger()
 
 
 def get_html(template_path: Path, title: str, css_definitions: str) -> Tuple[str, str]:
-    with open(template_path, "r") as f:
+    with open(template_path) as f:
         html_text = f.read()
         html_start, html_end = html_text.split("<!--PYREBALL_REPORT_CONTENTS-->")
         html_start = re.sub("<!--PYREBALL_PAGE_TITLE-->", title, html_start)
         html_start = re.sub(
             r"<!--PYREBALL_CSS_DEFINITIONS-->", css_definitions, html_start
         )
         return html_start, html_end
```

