# Comparing `tmp/dotbackup-1.2.0.tar.gz` & `tmp/dotbackup-1.2.1.tar.gz`

## Comparing `dotbackup-1.2.0.tar` & `dotbackup-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 dotbackup-1.2.0/dotbackup.1.adoc
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 dotbackup-1.2.0/dotsetup.1.adoc
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 dotbackup-1.2.0/requirements.txt
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dotbackup-1.2.0/setup.cfg
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dotbackup-1.2.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 dotbackup-1.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dotbackup-1.2.0/.github/workflows/style.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dotbackup-1.2.0/.github/workflows/test.yml
--rwxr-xr-x   0        0        0    12850 2020-02-02 00:00:00.000000 dotbackup-1.2.0/src/dotbackup.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/helper.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/misc_test.py
--rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/test_basic.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/test_complex_script.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/test_ignore.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/configs/basic.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/configs/complex_script.yml
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/configs/ignore.yml
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 dotbackup-1.2.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dotbackup-1.2.0/LICENSE
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 dotbackup-1.2.0/README.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 dotbackup-1.2.0/hatch_build.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 dotbackup-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 dotbackup-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 dotbackup-1.2.1/dotbackup.1.adoc
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 dotbackup-1.2.1/dotsetup.1.adoc
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 dotbackup-1.2.1/requirements.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dotbackup-1.2.1/setup.cfg
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dotbackup-1.2.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 dotbackup-1.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dotbackup-1.2.1/.github/workflows/style.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dotbackup-1.2.1/.github/workflows/test.yml
+-rwxr-xr-x   0        0        0    12850 2020-02-02 00:00:00.000000 dotbackup-1.2.1/src/dotbackup.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 dotbackup-1.2.1/tests/helper.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 dotbackup-1.2.1/tests/misc_test.py
+-rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 dotbackup-1.2.1/tests/test_basic.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 dotbackup-1.2.1/tests/test_complex_script.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 dotbackup-1.2.1/tests/test_ignore.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 dotbackup-1.2.1/tests/configs/basic.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 dotbackup-1.2.1/tests/configs/complex_script.yml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 dotbackup-1.2.1/tests/configs/ignore.yml
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 dotbackup-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dotbackup-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 dotbackup-1.2.1/README.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 dotbackup-1.2.1/hatch_build.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 dotbackup-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 dotbackup-1.2.1/PKG-INFO
```

### Comparing `dotbackup-1.2.0/dotbackup.1.adoc` & `dotbackup-1.2.1/dotbackup.1.adoc`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 == Name
 
 dotbackup - YAML config based backup utility
 
 == Synopsis
 
-*dotbackup* [-h|--help] [-c|--config _CONFIG_] [-l|--list] [-V|--version]
+*dotbackup* [-h|--help] [-c|--config _CONFIG_] [-l|--list] [-v|--version]
 [--clean] [--log-level _LOG_LEVEL_] [_APP_...]
 
 == Description
 
 Usually people maintain backup and setup scripts along with their dotfiles. But
 these scripts always contain a lot of repeat codes, and writing them is not fun!
 dotbackup and dotsetup are here to help.
@@ -40,15 +40,15 @@
 	Configuration files under _~/.config/dotbackup_ can also be specified by their
 	basenames, e.g., _~/.config/dotbackup/config.yml_ can be specified by
 	_config_. See _CONFIGURATION_ section for configuration definition.
 
 *-l, --list*::
 	List configured application and exit.
 
-*-V, --version*::
+*-v, --version*::
 	Print the version information and exit.
 
 *--clean*::
 	Do clean backup, i.e., delete old backup files before backup.
 
 *--log-level* _LOG_LEVEL_::
 	Set the log level, _LOG_LEVEL_ may be one of DEBUG, INFO, WARNING, ERROR,
```

### Comparing `dotbackup-1.2.0/dotsetup.1.adoc` & `dotbackup-1.2.1/dotsetup.1.adoc`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 == Name
 
 dotsetup - YAML config based backup utility
 
 == Synopsis
 
-*dotsetup* [-h|--help] [-c|--config _CONFIG_] [-l|--list] [-V|--version]
+*dotsetup* [-h|--help] [-c|--config _CONFIG_] [-l|--list] [-v|--version]
 [--clean] [--log-level _LOG_LEVEL_] [_APP_...]
 
 == Description
 
 Usually people maintain backup and setup scripts along with their dotfiles. But
 these scripts always contain a lot of repeat codes, and writing them is not fun!
 dotbackup and dotsetup are here to help.
@@ -40,15 +40,15 @@
 	Configuration files under _~/.config/dotbackup_ can also be specified by their
 	basenames, e.g., _~/.config/dotbackup/config.yml_ can be specified by
 	_config_. See _CONFIGURATION_ section for configuration definition.
 
 *-l, --list*::
 	List configured application and exit.
 
-*-V, --version*::
+*-v, --version*::
 	Print the version information and exit.
 
 *--clean*::
 	Do clean setup, i.e., delete old configuration files before setup.
 
 *--log-level* _LOG_LEVEL_::
 	Set the log level, _LOG_LEVEL_ may be one of DEBUG, INFO, WARNING, ERROR,
```

### Comparing `dotbackup-1.2.0/.github/workflows/lint.yml` & `dotbackup-1.2.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `dotbackup-1.2.0/.github/workflows/release.yml` & `dotbackup-1.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dotbackup-1.2.0/.github/workflows/test.yml` & `dotbackup-1.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dotbackup-1.2.0/src/dotbackup.py` & `dotbackup-1.2.1/src/dotbackup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 from argparse import ArgumentParser
 from logging import Formatter, Logger, LogRecord
 from pathlib import Path
 
 from ruamel.yaml import YAML
 
-__VERSION__ = "1.2.0"
+__VERSION__ = "1.2.1"
 
 
 class ColorFormatter(Formatter):
     def format(self, record: LogRecord) -> str:  # pragma: no cover
         template = "\x1b[%dm{}\x1b[00m"
 
         if record.levelno == logging.INFO:
@@ -124,15 +124,15 @@
         parser.add_argument(
             "-l",
             "--list",
             action="store_true",
             help="List configured applications and exit.",
         )
         parser.add_argument(
-            "-V",
+            "-v",
             "--version",
             action="store_true",
             help="Print the version number of dotbackup and exit.",
         )
         parser.add_argument(
             "--clean",
             action="store_true",
```

### Comparing `dotbackup-1.2.0/tests/helper.py` & `dotbackup-1.2.1/tests/helper.py`

 * *Files identical despite different names*

### Comparing `dotbackup-1.2.0/tests/misc_test.py` & `dotbackup-1.2.1/tests/misc_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     assert dotbackup.dotbackup() == 1
     assert dotbackup.dotsetup() == 1
     assert dotbackup.main(["backup"]) == 1
     assert dotbackup.main(["setup"]) == 1
 
 
-@pytest.mark.parametrize("option", ["-V", "--version"])
+@pytest.mark.parametrize("option", ["-v", "--version"])
 def test_version(option, capfd):
     with pytest.raises(SystemExit):
         dotbackup.dotbackup([option])
     assert capfd.readouterr().out == f"dotbackup {dotbackup.__VERSION__}\n"
     with pytest.raises(SystemExit):
         dotbackup.dotsetup([option])
     assert capfd.readouterr().out == f"dotbackup {dotbackup.__VERSION__}\n"
```

### Comparing `dotbackup-1.2.0/tests/test_basic.py` & `dotbackup-1.2.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `dotbackup-1.2.0/tests/test_ignore.py` & `dotbackup-1.2.1/tests/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dotbackup-1.2.0/tests/configs/basic.yml` & `dotbackup-1.2.1/tests/configs/basic.yml`

 * *Files identical despite different names*

### Comparing `dotbackup-1.2.0/.gitignore` & `dotbackup-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dotbackup-1.2.0/LICENSE` & `dotbackup-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dotbackup-1.2.0/README.md` & `dotbackup-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dotbackup-1.2.0/hatch_build.py` & `dotbackup-1.2.1/hatch_build.py`

 * *Files identical despite different names*

### Comparing `dotbackup-1.2.0/pyproject.toml` & `dotbackup-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dotbackup-1.2.0/PKG-INFO` & `dotbackup-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dotbackup
-Version: 1.2.0
+Version: 1.2.1
 Summary: YAML config based backup utility. Easy to use yet flexible. With a primary focus on dotfile backup & setup, but not limited to dotfiles.
 Project-URL: Homepage, https://github.com/jaxvanyang/dotbackup
 Project-URL: Source, https://github.com/jaxvanyang/dotbackup
 Project-URL: Repository, https://github.com/jaxvanyang/dotbackup.git
 Project-URL: Issues, https://github.com/jaxvanyang/dotbackup/issues
 Author-email: Jax Young <jaxvanyang@gmail.com>
 License-File: LICENSE
```

