# Comparing `tmp/markdown_exec-1.8.0.tar.gz` & `tmp/markdown_exec-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_exec-1.8.0.tar", last modified: Fri Jan  5 18:40:42 2024, max compression
+gzip compressed data, was "markdown_exec-1.8.1.tar", last modified: Mon Apr 15 16:53:26 2024, max compression
```

## Comparing `markdown_exec-1.8.0.tar` & `markdown_exec-1.8.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      754 2024-01-05 18:37:45.814372 markdown_exec-1.8.0/LICENSE
--rw-r--r--   0        0        0     3367 2024-01-05 18:37:48.791041 markdown_exec-1.8.0/README.md
--rw-r--r--   0        0        0     3185 2024-01-05 18:40:42.217986 markdown_exec-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     4366 2024-01-05 18:37:48.791041 markdown_exec-1.8.0/src/markdown_exec/__init__.py
--rw-r--r--   0        0        0     5657 2023-11-05 16:57:00.596754 markdown_exec-1.8.0/src/markdown_exec/ansi.css
--rw-r--r--   0        0        0     2710 2024-01-05 18:37:45.917705 markdown_exec-1.8.0/src/markdown_exec/debug.py
--rw-r--r--   0        0        0       51 2023-11-05 16:57:00.630087 markdown_exec-1.8.0/src/markdown_exec/formatters/__init__.py
--rw-r--r--   0        0        0     4761 2023-11-05 16:57:00.653419 markdown_exec-1.8.0/src/markdown_exec/formatters/base.py
--rw-r--r--   0        0        0      886 2023-11-05 16:57:00.653419 markdown_exec-1.8.0/src/markdown_exec/formatters/bash.py
--rw-r--r--   0        0        0      815 2023-11-05 16:57:00.670086 markdown_exec-1.8.0/src/markdown_exec/formatters/console.py
--rw-r--r--   0        0        0      276 2023-11-05 16:57:00.683419 markdown_exec-1.8.0/src/markdown_exec/formatters/markdown.py
--rw-r--r--   0        0        0      854 2023-11-05 16:57:00.706752 markdown_exec-1.8.0/src/markdown_exec/formatters/pycon.py
--rw-r--r--   0        0        0     2898 2024-01-05 17:48:17.990589 markdown_exec-1.8.0/src/markdown_exec/formatters/pyodide.py
--rw-r--r--   0        0        0     2406 2023-11-05 16:57:00.726752 markdown_exec-1.8.0/src/markdown_exec/formatters/python.py
--rw-r--r--   0        0        0      876 2023-11-05 16:57:00.726752 markdown_exec-1.8.0/src/markdown_exec/formatters/sh.py
--rw-r--r--   0        0        0     2046 2023-11-05 16:57:00.746751 markdown_exec-1.8.0/src/markdown_exec/formatters/tree.py
--rw-r--r--   0        0        0     2109 2023-11-05 16:57:00.760085 markdown_exec-1.8.0/src/markdown_exec/logger.py
--rw-r--r--   0        0        0     4701 2024-01-05 18:36:32.567651 markdown_exec-1.8.0/src/markdown_exec/mkdocs_plugin.py
--rw-r--r--   0        0        0     4291 2024-01-05 17:35:28.675090 markdown_exec-1.8.0/src/markdown_exec/processors.py
--rw-r--r--   0        0        0        0 2024-01-05 18:37:45.917705 markdown_exec-1.8.0/src/markdown_exec/py.typed
--rw-r--r--   0        0        0      849 2024-01-05 17:48:17.990589 markdown_exec-1.8.0/src/markdown_exec/pyodide.css
--rw-r--r--   0        0        0     3845 2024-01-05 17:48:17.993923 markdown_exec-1.8.0/src/markdown_exec/pyodide.js
--rw-r--r--   0        0        0     9459 2024-01-05 18:00:40.526407 markdown_exec-1.8.0/src/markdown_exec/rendering.py
--rw-r--r--   0        0        0      166 2024-01-05 18:37:45.924372 markdown_exec-1.8.0/tests/__init__.py
--rw-r--r--   0        0        0      635 2024-01-05 18:37:48.791041 markdown_exec-1.8.0/tests/conftest.py
--rw-r--r--   0        0        0     1443 2023-11-05 16:57:00.873417 markdown_exec-1.8.0/tests/test_base_formatter.py
--rw-r--r--   0        0        0     2080 2023-11-05 16:57:00.893416 markdown_exec-1.8.0/tests/test_converter.py
--rw-r--r--   0        0        0     4337 2023-11-05 16:57:00.916749 markdown_exec-1.8.0/tests/test_python.py
--rw-r--r--   0        0        0     2027 2023-11-05 16:57:00.936749 markdown_exec-1.8.0/tests/test_shell.py
--rw-r--r--   0        0        0     2335 2023-11-05 16:57:00.983415 markdown_exec-1.8.0/tests/test_toc.py
--rw-r--r--   0        0        0      488 2023-11-05 16:57:00.983415 markdown_exec-1.8.0/tests/test_tree.py
--rw-r--r--   0        0        0      995 2023-11-05 16:57:01.013414 markdown_exec-1.8.0/tests/test_validator.py
--rw-r--r--   0        0        0     4937 1970-01-01 00:00:00.000000 markdown_exec-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2024-03-20 15:30:02.179261 markdown_exec-1.8.1/LICENSE
+-rw-r--r--   0        0        0     3367 2024-03-20 15:30:04.979225 markdown_exec-1.8.1/README.md
+-rw-r--r--   0        0        0     1844 2024-04-15 16:53:26.659226 markdown_exec-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4366 2024-03-20 15:30:04.982558 markdown_exec-1.8.1/src/markdown_exec/__init__.py
+-rw-r--r--   0        0        0     8090 2024-04-15 16:45:33.050727 markdown_exec-1.8.1/src/markdown_exec/ansi.css
+-rw-r--r--   0        0        0     2840 2024-03-20 15:30:02.289260 markdown_exec-1.8.1/src/markdown_exec/debug.py
+-rw-r--r--   0        0        0       51 2023-11-05 16:57:00.630087 markdown_exec-1.8.1/src/markdown_exec/formatters/__init__.py
+-rw-r--r--   0        0        0     4761 2023-11-05 16:57:00.653419 markdown_exec-1.8.1/src/markdown_exec/formatters/base.py
+-rw-r--r--   0        0        0      886 2023-11-05 16:57:00.653419 markdown_exec-1.8.1/src/markdown_exec/formatters/bash.py
+-rw-r--r--   0        0        0      815 2023-11-05 16:57:00.670086 markdown_exec-1.8.1/src/markdown_exec/formatters/console.py
+-rw-r--r--   0        0        0      276 2023-11-05 16:57:00.683419 markdown_exec-1.8.1/src/markdown_exec/formatters/markdown.py
+-rw-r--r--   0        0        0      854 2023-11-05 16:57:00.706752 markdown_exec-1.8.1/src/markdown_exec/formatters/pycon.py
+-rw-r--r--   0        0        0     2898 2024-01-05 17:48:17.990589 markdown_exec-1.8.1/src/markdown_exec/formatters/pyodide.py
+-rw-r--r--   0        0        0     2406 2023-11-05 16:57:00.726752 markdown_exec-1.8.1/src/markdown_exec/formatters/python.py
+-rw-r--r--   0        0        0      876 2023-11-05 16:57:00.726752 markdown_exec-1.8.1/src/markdown_exec/formatters/sh.py
+-rw-r--r--   0        0        0     2046 2023-11-05 16:57:00.746751 markdown_exec-1.8.1/src/markdown_exec/formatters/tree.py
+-rw-r--r--   0        0        0     2109 2023-11-05 16:57:00.760085 markdown_exec-1.8.1/src/markdown_exec/logger.py
+-rw-r--r--   0        0        0     4701 2024-01-05 18:36:32.567651 markdown_exec-1.8.1/src/markdown_exec/mkdocs_plugin.py
+-rw-r--r--   0        0        0     4291 2024-01-05 17:35:28.675090 markdown_exec-1.8.1/src/markdown_exec/processors.py
+-rw-r--r--   0        0        0        0 2024-03-20 15:30:02.292593 markdown_exec-1.8.1/src/markdown_exec/py.typed
+-rw-r--r--   0        0        0      849 2024-01-05 17:48:17.990589 markdown_exec-1.8.1/src/markdown_exec/pyodide.css
+-rw-r--r--   0        0        0     3845 2024-01-05 17:48:17.993923 markdown_exec-1.8.1/src/markdown_exec/pyodide.js
+-rw-r--r--   0        0        0     9459 2024-01-05 18:00:40.526407 markdown_exec-1.8.1/src/markdown_exec/rendering.py
+-rw-r--r--   0        0        0      166 2024-03-20 15:30:02.299260 markdown_exec-1.8.1/tests/__init__.py
+-rw-r--r--   0        0        0      635 2024-03-20 15:30:04.982558 markdown_exec-1.8.1/tests/conftest.py
+-rw-r--r--   0        0        0     1443 2023-11-05 16:57:00.873417 markdown_exec-1.8.1/tests/test_base_formatter.py
+-rw-r--r--   0        0        0     2080 2023-11-05 16:57:00.893416 markdown_exec-1.8.1/tests/test_converter.py
+-rw-r--r--   0        0        0     4337 2023-11-05 16:57:00.916749 markdown_exec-1.8.1/tests/test_python.py
+-rw-r--r--   0        0        0     2027 2023-11-05 16:57:00.936749 markdown_exec-1.8.1/tests/test_shell.py
+-rw-r--r--   0        0        0     2335 2023-11-05 16:57:00.983415 markdown_exec-1.8.1/tests/test_toc.py
+-rw-r--r--   0        0        0      488 2023-11-05 16:57:00.983415 markdown_exec-1.8.1/tests/test_tree.py
+-rw-r--r--   0        0        0      995 2023-11-05 16:57:01.013414 markdown_exec-1.8.1/tests/test_validator.py
+-rw-r--r--   0        0        0     4954 1970-01-01 00:00:00.000000 markdown_exec-1.8.1/PKG-INFO
```

### Comparing `markdown_exec-1.8.0/LICENSE` & `markdown_exec-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/README.md` & `markdown_exec-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/__init__.py` & `markdown_exec-1.8.1/src/markdown_exec/__init__.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/ansi.css` & `markdown_exec-1.8.1/src/markdown_exec/ansi.css`

 * *Files 19% similar despite different names*

```diff
@@ -11,57 +11,65 @@
     --ansi-cyan: #8be9fd;
     --ansi-black: #282a36;
     --ansi-white: #f8f8f2;
 }
 
 .-Color-Green,
 .-Color-Faint-Green,
-.-Color-Bold-Green {
+.-Color-Bold-Green,
+.-Color-BrightGreen {
     color: var(--ansi-green);
 }
 
 .-Color-Red,
 .-Color-Faint-Red,
-.-Color-Bold-Red {
+.-Color-Bold-Red,
+.-Color-BrightRed {
     color: var(--ansi-red);
 }
 
 .-Color-Yellow,
 .-Color-Faint-Yellow,
-.-Color-Bold-Yellow {
+.-Color-Bold-Yellow,
+.-Color-BrightYellow {
     color: var(--ansi-yellow);
 }
 
 .-Color-Blue,
 .-Color-Faint-Blue,
-.-Color-Bold-Blue {
+.-Color-Bold-Blue,
+.-Color-BrightBlue {
     color: var(--ansi-blue);
 }
 
 .-Color-Magenta,
 .-Color-Faint-Magenta,
-.-Color-Bold-Magenta {
+.-Color-Bold-Magenta,
+.-Color-BrightMagenta {
     color: var(--ansi-magenta);
 }
 
 .-Color-Cyan,
 .-Color-Faint-Cyan,
-.-Color-Bold-Cyan {
+.-Color-Bold-Cyan,
+.-Color-BrightCyan {
     color: var(--ansi-cyan);
 }
 
 .-Color-White,
 .-Color-Faint-White,
-.-Color-Bold-White {
+.-Color-Bold-White,
+.-Color-BrightWhite {
     color: var(--ansi-white);
 }
 
 .-Color-Black,
 .-Color-Faint-Black,
-.-Color-Bold-Black {
+.-Color-Bold-Black,
+.-Color-BrightBlack {
     color: var(--ansi-black);
 }
 
 .-Color-Faint {
     opacity: 0.5;
 }
 
@@ -69,195 +77,276 @@
     font-weight: bold;
 }
 
 .-Color-BGBlack,
 .-Color-Black-BGBlack,
 .-Color-Blue-BGBlack,
 .-Color-Bold-BGBlack,
+.-Color-BrightBGBlack,
 .-Color-Bold-Black-BGBlack,
+.-Color-BrightBlack-BGBlack,
 .-Color-Bold-Green-BGBlack,
+.-Color-BrightGreen-BGBlack,
 .-Color-Bold-Cyan-BGBlack,
+.-Color-BrightCyan-BGBlack,
 .-Color-Bold-Blue-BGBlack,
+.-Color-BrightBlue-BGBlack,
 .-Color-Bold-Magenta-BGBlack,
+.-Color-BrightMagenta-BGBlack,
 .-Color-Bold-Red-BGBlack,
+.-Color-BrightRed-BGBlack,
 .-Color-Bold-White-BGBlack,
+.-Color-BrightWhite-BGBlack,
 .-Color-Bold-Yellow-BGBlack,
+.-Color-BrightYellow-BGBlack,
 .-Color-Cyan-BGBlack,
 .-Color-Green-BGBlack,
 .-Color-Magenta-BGBlack,
 .-Color-Red-BGBlack,
 .-Color-White-BGBlack,
 .-Color-Yellow-BGBlack {
     background-color: var(--ansi-black);
 }
 
 .-Color-BGRed,
 .-Color-Black-BGRed,
 .-Color-Blue-BGRed,
 .-Color-Bold-BGRed,
+.-Color-BrightBGRed,
 .-Color-Bold-Black-BGRed,
+.-Color-BrightBlack-BGRed,
 .-Color-Bold-Green-BGRed,
+.-Color-BrightGreen-BGRed,
 .-Color-Bold-Cyan-BGRed,
+.-Color-BrightCyan-BGRed,
 .-Color-Bold-Blue-BGRed,
+.-Color-BrightBlue-BGRed,
 .-Color-Bold-Magenta-BGRed,
+.-Color-BrightMagenta-BGRed,
 .-Color-Bold-Red-BGRed,
+.-Color-BrightRed-BGRed,
 .-Color-Bold-White-BGRed,
+.-Color-BrightWhite-BGRed,
 .-Color-Bold-Yellow-BGRed,
+.-Color-BrightYellow-BGRed,
 .-Color-Cyan-BGRed,
 .-Color-Green-BGRed,
 .-Color-Magenta-BGRed,
 .-Color-Red-BGRed,
 .-Color-White-BGRed,
 .-Color-Yellow-BGRed {
     background-color: var(--ansi-red);
 }
 
 .-Color-BGGreen,
 .-Color-Black-BGGreen,
 .-Color-Blue-BGGreen,
 .-Color-Bold-BGGreen,
+.-Color-BrightBGGreen,
 .-Color-Bold-Black-BGGreen,
+.-Color-BrightBlack-BGGreen,
 .-Color-Bold-Green-BGGreen,
+.-Color-BrightGreen-BGGreen,
 .-Color-Bold-Cyan-BGGreen,
+.-Color-BrightCyan-BGGreen,
 .-Color-Bold-Blue-BGGreen,
+.-Color-BrightBlue-BGGreen,
 .-Color-Bold-Magenta-BGGreen,
+.-Color-BrightMagenta-BGGreen,
 .-Color-Bold-Red-BGGreen,
+.-Color-BrightRed-BGGreen,
 .-Color-Bold-White-BGGreen,
+.-Color-BrightWhite-BGGreen,
 .-Color-Bold-Yellow-BGGreen,
+.-Color-BrightYellow-BGGreen,
 .-Color-Cyan-BGGreen,
 .-Color-Green-BGGreen,
 .-Color-Magenta-BGGreen,
 .-Color-Red-BGGreen,
 .-Color-White-BGGreen,
 .-Color-Yellow-BGGreen {
     background-color: var(--ansi-green);
 }
 
 .-Color-BGYellow,
 .-Color-Black-BGYellow,
 .-Color-Blue-BGYellow,
 .-Color-Bold-BGYellow,
+.-Color-BrightBGYellow,
 .-Color-Bold-Black-BGYellow,
+.-Color-BrightBlack-BGYellow,
 .-Color-Bold-Green-BGYellow,
+.-Color-BrightGreen-BGYellow,
 .-Color-Bold-Cyan-BGYellow,
+.-Color-BrightCyan-BGYellow,
 .-Color-Bold-Blue-BGYellow,
+.-Color-BrightBlue-BGYellow,
 .-Color-Bold-Magenta-BGYellow,
+.-Color-BrightMagenta-BGYellow,
 .-Color-Bold-Red-BGYellow,
+.-Color-BrightRed-BGYellow,
 .-Color-Bold-White-BGYellow,
+.-Color-BrightWhite-BGYellow,
 .-Color-Bold-Yellow-BGYellow,
+.-Color-BrightYellow-BGYellow,
 .-Color-Cyan-BGYellow,
 .-Color-Green-BGYellow,
 .-Color-Magenta-BGYellow,
 .-Color-Red-BGYellow,
 .-Color-White-BGYellow,
 .-Color-Yellow-BGYellow {
     background-color: var(--ansi-yellow);
 }
 
 .-Color-BGBlue,
 .-Color-Black-BGBlue,
 .-Color-Blue-BGBlue,
 .-Color-Bold-BGBlue,
+.-Color-BrightBGBlue,
 .-Color-Bold-Black-BGBlue,
+.-Color-BrightBlack-BGBlue,
 .-Color-Bold-Green-BGBlue,
+.-Color-BrightGreen-BGBlue,
 .-Color-Bold-Cyan-BGBlue,
+.-Color-BrightCyan-BGBlue,
 .-Color-Bold-Blue-BGBlue,
+.-Color-BrightBlue-BGBlue,
 .-Color-Bold-Magenta-BGBlue,
+.-Color-BrightMagenta-BGBlue,
 .-Color-Bold-Red-BGBlue,
+.-Color-BrightRed-BGBlue,
 .-Color-Bold-White-BGBlue,
+.-Color-BrightWhite-BGBlue,
 .-Color-Bold-Yellow-BGBlue,
+.-Color-BrightYellow-BGBlue,
 .-Color-Cyan-BGBlue,
 .-Color-Green-BGBlue,
 .-Color-Magenta-BGBlue,
 .-Color-Red-BGBlue,
 .-Color-White-BGBlue,
 .-Color-Yellow-BGBlue {
     background-color: var(--ansi-blue);
 }
 
 .-Color-BGMagenta,
 .-Color-Black-BGMagenta,
 .-Color-Blue-BGMagenta,
 .-Color-Bold-BGMagenta,
+.-Color-BrightBGMagenta,
 .-Color-Bold-Black-BGMagenta,
+.-Color-BrightBlack-BGMagenta,
 .-Color-Bold-Green-BGMagenta,
+.-Color-BrightGreen-BGMagenta,
 .-Color-Bold-Cyan-BGMagenta,
+.-Color-BrightCyan-BGMagenta,
 .-Color-Bold-Blue-BGMagenta,
+.-Color-BrightBlue-BGMagenta,
 .-Color-Bold-Magenta-BGMagenta,
+.-Color-BrightMagenta-BGMagenta,
 .-Color-Bold-Red-BGMagenta,
+.-Color-BrightRed-BGMagenta,
 .-Color-Bold-White-BGMagenta,
+.-Color-BrightWhite-BGMagenta,
 .-Color-Bold-Yellow-BGMagenta,
+.-Color-BrightYellow-BGMagenta,
 .-Color-Cyan-BGMagenta,
 .-Color-Green-BGMagenta,
 .-Color-Magenta-BGMagenta,
 .-Color-Red-BGMagenta,
 .-Color-White-BGMagenta,
 .-Color-Yellow-BGMagenta {
     background-color: var(--ansi-magenta);
 }
 
 .-Color-BGCyan,
 .-Color-Black-BGCyan,
 .-Color-Blue-BGCyan,
 .-Color-Bold-BGCyan,
+.-Color-BrightBGCyan,
 .-Color-Bold-Black-BGCyan,
+.-Color-BrightBlack-BGCyan,
 .-Color-Bold-Green-BGCyan,
+.-Color-BrightGreen-BGCyan,
 .-Color-Bold-Cyan-BGCyan,
+.-Color-BrightCyan-BGCyan,
 .-Color-Bold-Blue-BGCyan,
+.-Color-BrightBlue-BGCyan,
 .-Color-Bold-Magenta-BGCyan,
+.-Color-BrightMagenta-BGCyan,
 .-Color-Bold-Red-BGCyan,
+.-Color-BrightRed-BGCyan,
 .-Color-Bold-White-BGCyan,
+.-Color-BrightWhite-BGCyan,
 .-Color-Bold-Yellow-BGCyan,
+.-Color-BrightYellow-BGCyan,
 .-Color-Cyan-BGCyan,
 .-Color-Green-BGCyan,
 .-Color-Magenta-BGCyan,
 .-Color-Red-BGCyan,
 .-Color-White-BGCyan,
 .-Color-Yellow-BGCyan {
     background-color: var(--ansi-cyan);
 }
 
 .-Color-BGWhite,
 .-Color-Black-BGWhite,
 .-Color-Blue-BGWhite,
 .-Color-Bold-BGWhite,
+.-Color-BrightBGWhite,
 .-Color-Bold-Black-BGWhite,
+.-Color-BrightBlack-BGWhite,
 .-Color-Bold-Green-BGWhite,
+.-Color-BrightGreen-BGWhite,
 .-Color-Bold-Cyan-BGWhite,
+.-Color-BrightCyan-BGWhite,
 .-Color-Bold-Blue-BGWhite,
+.-Color-BrightBlue-BGWhite,
 .-Color-Bold-Magenta-BGWhite,
+.-Color-BrightMagenta-BGWhite,
 .-Color-Bold-Red-BGWhite,
+.-Color-BrightRed-BGWhite,
 .-Color-Bold-White-BGWhite,
+.-Color-BrightWhite-BGWhite,
 .-Color-Bold-Yellow-BGWhite,
+.-Color-BrightYellow-BGWhite,
 .-Color-Cyan-BGWhite,
 .-Color-Green-BGWhite,
 .-Color-Magenta-BGWhite,
 .-Color-Red-BGWhite,
 .-Color-White-BGWhite,
 .-Color-Yellow-BGWhite {
     background-color: var(--ansi-white);
 }
 
 .-Color-Black,
 .-Color-Bold-Black,
+.-Color-BrightBlack,
 .-Color-Black-BGBlack,
 .-Color-Bold-Black-BGBlack,
+.-Color-BrightBlack-BGBlack,
 .-Color-Black-BGGreen,
 .-Color-Red-BGRed,
 .-Color-Bold-Red-BGRed,
+.-Color-BrightRed-BGRed,
 .-Color-Bold-Blue-BGBlue,
+.-Color-BrightBlue-BGBlue,
 .-Color-Blue-BGBlue {
     text-shadow: 0 0 1px var(--ansi-white);
 }
 
 .-Color-Bold-Cyan-BGCyan,
+.-Color-BrightCyan-BGCyan,
 .-Color-Bold-Magenta-BGMagenta,
+.-Color-BrightMagenta-BGMagenta,
 .-Color-Bold-White,
+.-Color-BrightWhite,
 .-Color-Bold-Yellow-BGYellow,
+.-Color-BrightYellow-BGYellow,
 .-Color-Bold-Green-BGGreen,
+.-Color-BrightGreen-BGGreen,
 .-Color-Cyan-BGCyan,
 .-Color-Cyan-BGGreen,
 .-Color-Green-BGCyan,
 .-Color-Green-BGGreen,
 .-Color-Magenta-BGMagenta,
 .-Color-White,
 .-Color-White-BGWhite,
```

### Comparing `markdown_exec-1.8.0/src/markdown_exec/debug.py` & `markdown_exec-1.8.1/src/markdown_exec/debug.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 class Environment:
     """Dataclass to store environment information."""
 
     interpreter_name: str
     """Python interpreter name."""
     interpreter_version: str
     """Python interpreter version."""
+    interpreter_path: str
+    """Path to Python executable."""
     platform: str
     """Operating System."""
     packages: list[Package]
     """Installed packages."""
     variables: list[Variable]
     """Environment variables."""
 
@@ -79,25 +81,26 @@
     """
     py_name, py_version = _interpreter_name_version()
     packages = ["markdown-exec"]
     variables = ["PYTHONPATH", *[var for var in os.environ if var.startswith("MARKDOWN_EXEC")]]
     return Environment(
         interpreter_name=py_name,
         interpreter_version=py_version,
+        interpreter_path=sys.executable,
         platform=platform.platform(),
         variables=[Variable(var, val) for var in variables if (val := os.getenv(var))],
         packages=[Package(pkg, get_version(pkg)) for pkg in packages],
     )
 
 
 def print_debug_info() -> None:
     """Print debug/environment information."""
     info = get_debug_info()
     print(f"- __System__: {info.platform}")
-    print(f"- __Python__: {info.interpreter_name} {info.interpreter_version}")
+    print(f"- __Python__: {info.interpreter_name} {info.interpreter_version} ({info.interpreter_path})")
     print("- __Environment variables__:")
     for var in info.variables:
         print(f"  - `{var.name}`: `{var.value}`")
     print("- __Installed packages__:")
     for pkg in info.packages:
         print(f"  - `{pkg.name}` v{pkg.version}")
```

### Comparing `markdown_exec-1.8.0/src/markdown_exec/formatters/base.py` & `markdown_exec-1.8.1/src/markdown_exec/formatters/base.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/formatters/bash.py` & `markdown_exec-1.8.1/src/markdown_exec/formatters/bash.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/formatters/console.py` & `markdown_exec-1.8.1/src/markdown_exec/formatters/console.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/formatters/pycon.py` & `markdown_exec-1.8.1/src/markdown_exec/formatters/pycon.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/formatters/pyodide.py` & `markdown_exec-1.8.1/src/markdown_exec/formatters/pyodide.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/formatters/python.py` & `markdown_exec-1.8.1/src/markdown_exec/formatters/python.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/formatters/sh.py` & `markdown_exec-1.8.1/src/markdown_exec/formatters/sh.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/formatters/tree.py` & `markdown_exec-1.8.1/src/markdown_exec/formatters/tree.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/logger.py` & `markdown_exec-1.8.1/src/markdown_exec/logger.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/mkdocs_plugin.py` & `markdown_exec-1.8.1/src/markdown_exec/mkdocs_plugin.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/processors.py` & `markdown_exec-1.8.1/src/markdown_exec/processors.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/pyodide.css` & `markdown_exec-1.8.1/src/markdown_exec/pyodide.css`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/pyodide.js` & `markdown_exec-1.8.1/src/markdown_exec/pyodide.js`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/src/markdown_exec/rendering.py` & `markdown_exec-1.8.1/src/markdown_exec/rendering.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/tests/conftest.py` & `markdown_exec-1.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/tests/test_base_formatter.py` & `markdown_exec-1.8.1/tests/test_base_formatter.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/tests/test_converter.py` & `markdown_exec-1.8.1/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/tests/test_python.py` & `markdown_exec-1.8.1/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/tests/test_shell.py` & `markdown_exec-1.8.1/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/tests/test_toc.py` & `markdown_exec-1.8.1/tests/test_toc.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/tests/test_validator.py` & `markdown_exec-1.8.1/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.0/PKG-INFO` & `markdown_exec-1.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: markdown-exec
-Version: 1.8.0
+Version: 1.8.1
 Summary: Utilities to execute code blocks in Markdown files.
-Keywords: markdown python exec shell bash mkdocs
-Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
+Keywords: markdown,python,exec,shell,bash,mkdocs
+Author-Email: =?utf-8?q?Timoth=C3=A9e_Mazzucotelli?= <dev@pawamoy.fr>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

