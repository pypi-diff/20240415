# Comparing `tmp/git-clog-0.2.5.tar.gz` & `tmp/git-clog-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/git-clog-0.2.5.tar", last modified: Sat Apr 25 10:33:03 2020, max compression
+gzip compressed data, was "git-clog-0.3.0.tar", last modified: Mon Apr 15 13:13:40 2024, max compression
```

## Comparing `git-clog-0.2.5.tar` & `git-clog-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-25 10:33:03.425392 git-clog-0.2.5/
--rw-rw-rw-   0 root         (0) root         (0)     1053 2020-04-25 10:32:56.000000 git-clog-0.2.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       57 2020-04-25 10:32:56.000000 git-clog-0.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2361 2020-04-25 10:33:03.425392 git-clog-0.2.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      838 2020-04-25 10:32:56.000000 git-clog-0.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-25 10:33:03.425392 git-clog-0.2.5/git_clog.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2361 2020-04-25 10:33:03.000000 git-clog-0.2.5/git_clog.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      228 2020-04-25 10:33:03.000000 git-clog-0.2.5/git_clog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-04-25 10:33:03.000000 git-clog-0.2.5/git_clog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2020-04-25 10:33:03.000000 git-clog-0.2.5/git_clog.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2020-04-25 10:33:03.000000 git-clog-0.2.5/git_clog.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     5308 2020-04-25 10:32:56.000000 git-clog-0.2.5/git_clog.py
--rw-rw-rw-   0 root         (0) root         (0)   182629 2020-04-25 10:32:56.000000 git-clog-0.2.5/screenshot.png
--rw-r--r--   0 root         (0) root         (0)       38 2020-04-25 10:33:03.425392 git-clog-0.2.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2063 2020-04-25 10:32:56.000000 git-clog-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:13:40.152521 git-clog-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2024-04-15 13:13:31.000000 git-clog-0.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-04-15 13:13:31.000000 git-clog-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2208 2024-04-15 13:13:40.152521 git-clog-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-04-15 13:13:31.000000 git-clog-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:13:40.152521 git-clog-0.3.0/git_clog.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2208 2024-04-15 13:13:40.000000 git-clog-0.3.0/git_clog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      243 2024-04-15 13:13:40.000000 git-clog-0.3.0/git_clog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 13:13:40.000000 git-clog-0.3.0/git_clog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-15 13:13:40.000000 git-clog-0.3.0/git_clog.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-15 13:13:40.000000 git-clog-0.3.0/git_clog.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     6487 2024-04-15 13:13:31.000000 git-clog-0.3.0/git_clog.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-04-15 13:13:31.000000 git-clog-0.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)   182629 2024-04-15 13:13:31.000000 git-clog-0.3.0/screenshot.png
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 13:13:40.152521 git-clog-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2060 2024-04-15 13:13:31.000000 git-clog-0.3.0/setup.py
```

### Comparing `git-clog-0.2.5/LICENSE` & `git-clog-0.3.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2019 Ingo Heimbach
+Copyright 2019 Ingo Meyer
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `git-clog-0.2.5/PKG-INFO` & `git-clog-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,16 @@
 Metadata-Version: 2.1
 Name: git-clog
-Version: 0.2.5
+Version: 0.3.0
 Summary: git-clog outputs the commit graph of the current Git repository and colorizes commit symbols by interpreting the first six commit hash digits as an RGB color value.
-Home-page: https://github.com/IngoHeimbach/git-clog
-Author: Ingo Heimbach
-Author-email: IJ_H@gmx.de
+Home-page: https://github.com/IngoMeyer441/git-clog
+Author: Ingo Meyer
+Author-email: IJ_M@gmx.de
 License: MIT
-Description: # Git colorlog
-        
-        ## Introduction
-        
-        `git clog` outputs the commit graph of the current Git repository and colorizes commit symbols by interpreting the first
-        six commit hash digits as an RGB color value:
-        
-        ![git clog screenshot](https://raw.githubusercontent.com/IngoHeimbach/git-clog/master/screenshot.png)
-        
-        **Important note**: You need a [terminal with true color support](https://gist.github.com/XVilka/8346728).
-        
-        ## Installation and usage
-        
-        `git clog` is [available on PyPI](https://pypi.org/project/git-clog/) and can be installed with `pip`:
-        
-        ```bash
-        python3 -m pip install git-clog
-        ```
-        
-        If you use Arch Linux or one of its derivatives, you can also install `git-clog` from the
-        [AUR](https://aur.archlinux.org/packages/git-clog/):
-        
-        ```bash
-        yay -S git-clog
-        ```
-        
-        After the installation, call
-        
-        ```bash
-        git clog
-        ```
-        
-        within a Git repository.
-        
 Keywords: git
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
@@ -57,7 +22,45 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Git colorlog
+
+## Introduction
+
+`git clog` outputs the commit graph of the current Git repository and colorizes commit symbols by interpreting the first
+six commit hash digits as an RGB color value:
+
+![git clog screenshot](https://raw.githubusercontent.com/IngoMeyer441/git-clog/master/screenshot.png)
+
+Additionally, signed commits are displayed with a check mark (valid), cross mark (invalid), or a question mark
+(unknown).
+
+**Important note**: You need a [terminal with true color support](https://gist.github.com/XVilka/8346728).
+
+## Installation and usage
+
+`git clog` is [available on PyPI](https://pypi.org/project/git-clog/) and can be installed with `pip`:
+
+```bash
+python3 -m pip install git-clog
+```
+
+If you use Arch Linux or one of its derivatives, you can also install `git-clog` from the
+[AUR](https://aur.archlinux.org/packages/git-clog/):
+
+```bash
+yay -S git-clog
+```
+
+After the installation, call
+
+```bash
+git clog
+```
+
+within a Git repository.
```

### Comparing `git-clog-0.2.5/README.md` & `git-clog-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Git colorlog
 
 ## Introduction
 
 `git clog` outputs the commit graph of the current Git repository and colorizes commit symbols by interpreting the first
 six commit hash digits as an RGB color value:
 
-![git clog screenshot](https://raw.githubusercontent.com/IngoHeimbach/git-clog/master/screenshot.png)
+![git clog screenshot](https://raw.githubusercontent.com/IngoMeyer441/git-clog/master/screenshot.png)
+
+Additionally, signed commits are displayed with a check mark (valid), cross mark (invalid), or a question mark
+(unknown).
 
 **Important note**: You need a [terminal with true color support](https://gist.github.com/XVilka/8346728).
 
 ## Installation and usage
 
 `git clog` is [available on PyPI](https://pypi.org/project/git-clog/) and can be installed with `pip`:
```

### Comparing `git-clog-0.2.5/git_clog.egg-info/PKG-INFO` & `git-clog-0.3.0/git_clog.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,16 @@
 Metadata-Version: 2.1
 Name: git-clog
-Version: 0.2.5
+Version: 0.3.0
 Summary: git-clog outputs the commit graph of the current Git repository and colorizes commit symbols by interpreting the first six commit hash digits as an RGB color value.
-Home-page: https://github.com/IngoHeimbach/git-clog
-Author: Ingo Heimbach
-Author-email: IJ_H@gmx.de
+Home-page: https://github.com/IngoMeyer441/git-clog
+Author: Ingo Meyer
+Author-email: IJ_M@gmx.de
 License: MIT
-Description: # Git colorlog
-        
-        ## Introduction
-        
-        `git clog` outputs the commit graph of the current Git repository and colorizes commit symbols by interpreting the first
-        six commit hash digits as an RGB color value:
-        
-        ![git clog screenshot](https://raw.githubusercontent.com/IngoHeimbach/git-clog/master/screenshot.png)
-        
-        **Important note**: You need a [terminal with true color support](https://gist.github.com/XVilka/8346728).
-        
-        ## Installation and usage
-        
-        `git clog` is [available on PyPI](https://pypi.org/project/git-clog/) and can be installed with `pip`:
-        
-        ```bash
-        python3 -m pip install git-clog
-        ```
-        
-        If you use Arch Linux or one of its derivatives, you can also install `git-clog` from the
-        [AUR](https://aur.archlinux.org/packages/git-clog/):
-        
-        ```bash
-        yay -S git-clog
-        ```
-        
-        After the installation, call
-        
-        ```bash
-        git clog
-        ```
-        
-        within a Git repository.
-        
 Keywords: git
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
@@ -57,7 +22,45 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Git colorlog
+
+## Introduction
+
+`git clog` outputs the commit graph of the current Git repository and colorizes commit symbols by interpreting the first
+six commit hash digits as an RGB color value:
+
+![git clog screenshot](https://raw.githubusercontent.com/IngoMeyer441/git-clog/master/screenshot.png)
+
+Additionally, signed commits are displayed with a check mark (valid), cross mark (invalid), or a question mark
+(unknown).
+
+**Important note**: You need a [terminal with true color support](https://gist.github.com/XVilka/8346728).
+
+## Installation and usage
+
+`git clog` is [available on PyPI](https://pypi.org/project/git-clog/) and can be installed with `pip`:
+
+```bash
+python3 -m pip install git-clog
+```
+
+If you use Arch Linux or one of its derivatives, you can also install `git-clog` from the
+[AUR](https://aur.archlinux.org/packages/git-clog/):
+
+```bash
+yay -S git-clog
+```
+
+After the installation, call
+
+```bash
+git clog
+```
+
+within a Git repository.
```

### Comparing `git-clog-0.2.5/git_clog.py` & `git-clog-0.3.0/git_clog.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import os
 import pty
 import re
 import subprocess
 import sys
 from typing import Iterator, List, Optional, Tuple  # noqa: F401  # pylint: disable=unused-import
 
-__author__ = "Ingo Heimbach"
-__email__ = "IJ_H@gmx.de"
+__author__ = "Ingo Meyer"
+__email__ = "IJ_M@gmx.de"
 __license__ = "MIT"
-__version_info__ = (0, 2, 5)
+__version_info__ = (0, 3, 0)
 __version__ = ".".join(map(str, __version_info__))
 
 BLOCK_SIZE = 1024
 COMMIT_CHAR_ASCII = "*"
 COMMIT_CHAR_UNICODE = "●"
 
 
@@ -75,15 +75,16 @@
         pager_options = ["-R"]
     return [pager] + pager_options
 
 
 def gen_git_log() -> Iterator[str]:
     master_fd, slave_fd = pty.openpty()
     git_log_process = subprocess.Popen(
-        ["git", "--no-pager", "log", "--color=always", "--all", "--decorate", "--graph", "--oneline"], stdout=slave_fd
+        ["git", "--no-pager", "log", "--color=always", "--all", "--graph", "--format=%C(auto)%h%d %s %G?"],
+        stdout=slave_fd,
     )
     os.close(slave_fd)  # otherwise read from `master_fd` will wait forever
     byte_block = b""
     try:
         while True:
             try:
                 current_bytes = os.read(master_fd, BLOCK_SIZE)
@@ -105,34 +106,71 @@
         yield decode(byte_block)
     returncode = git_log_process.wait()
     if returncode != 0:
         raise GitLogError(returncode)
 
 
 def gen_colorized_git_log_output(git_log_iterator: Iterator[str]) -> Iterator[str]:
+    def colorize_sign_state(sign_state: str) -> str:
+        sign_to_escape_code = {
+            "G": "\x1b[32m",
+            "B": "\x1b[31m",
+            "U": "\x1b[33m",
+            "X": "\x1b[31m",
+            "Y": "\x1b[31m",
+            "R": "\x1b[31m",
+            "E": "\x1b[33m",
+            "N": "",
+        }
+        sign_to_text = {
+            "G": "✓",
+            "B": "✗ (bad)",
+            "U": "? (unknown validity)",
+            "X": "✗ (expired)",
+            "Y": "✗ (expired key)",
+            "R": "✗ (revoked key)",
+            "E": "? (missing key)",
+            "N": "",
+        }
+        if sign_to_text.get(sign_state) == "":
+            return ""
+        escape_code = sign_to_escape_code.get(sign_state, "")
+        sign_text = sign_to_text.get(sign_state)
+        if sign_text is None:
+            return sign_state
+        return "".join(
+            (
+                escape_code,
+                sign_text[:1],
+                "\x1b[m",
+                "".join(("\x1b[90m", sign_text[1:], "\x1b[m")) if len(sign_text) > 1 else "",
+            )
+        )
+
     commit_char = COMMIT_CHAR_UNICODE if is_locale_utf8() else COMMIT_CHAR_ASCII
-    line_regex = re.compile(r"([^\*]*)\*([^()]*\x1b[^m]*m)([0-9a-f]+)(\x1b[^m]*m.*)")
+    line_regex = re.compile(r"([^\*]*)\*([^()]*\x1b[^m]*m)([0-9a-f]+)(\x1b[^m]*m.*)(.)$")
     for line in git_log_iterator:
         line = line.rstrip()
         match_obj = line_regex.match(line)
         if match_obj is not None:
-            line_start, before_commit_hash, commit_hash, rest_of_line = match_obj.groups()
+            line_start, before_commit_hash, commit_hash, rest_of_line, sign_state = match_obj.groups()
             color_rgb_tuple = tuple(int(commit_hash[i : i + 2], base=16) for i in range(0, 6, 2))
             true_color_escape_sequence = "\x1b[38;2;{r:d};{g:d};{b:d}m".format(
                 r=color_rgb_tuple[0], g=color_rgb_tuple[1], b=color_rgb_tuple[2]
             )
             colored_line = "".join(
                 [
                     line_start,
                     true_color_escape_sequence,
                     commit_char,
                     "\x1b[m",
                     before_commit_hash,
                     commit_hash,
                     rest_of_line,
+                    colorize_sign_state(sign_state),
                 ]
             )
             yield colored_line
         else:
             yield line
```

### Comparing `git-clog-0.2.5/screenshot.png` & `git-clog-0.3.0/screenshot.png`

 * *Files identical despite different names*

### Comparing `git-clog-0.2.5/setup.py` & `git-clog-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 
 setup(
     name="git-clog",
     version=version,
     py_modules=["git_clog"],
     python_requires="~=3.3",
     entry_points={"console_scripts": ["git-clog = git_clog:main"]},
-    author="Ingo Heimbach",
-    author_email="IJ_H@gmx.de",
+    author="Ingo Meyer",
+    author_email="IJ_M@gmx.de",
     description=(
         "git-clog outputs the commit graph of the current Git repository and colorizes commit symbols by "
         "interpreting the first six commit hash digits as an RGB color value."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
-    url="https://github.com/IngoHeimbach/git-clog",
+    url="https://github.com/IngoMeyer441/git-clog",
     keywords=["git"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
```

