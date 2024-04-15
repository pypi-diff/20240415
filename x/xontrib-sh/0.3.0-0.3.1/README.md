# Comparing `tmp/xontrib-sh-0.3.0.tar.gz` & `tmp/xontrib_sh-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xontrib-sh-0.3.0.tar", last modified: Fri Mar 19 16:21:25 2021, max compression
+gzip compressed data, was "xontrib_sh-0.3.1.tar", last modified: Mon Apr 15 09:20:59 2024, max compression
```

## Comparing `xontrib-sh-0.3.0.tar` & `xontrib_sh-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-19 16:21:25.952780 xontrib-sh-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-03-19 16:21:17.000000 xontrib-sh-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-19 16:21:17.000000 xontrib-sh-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2021-03-19 16:21:25.952780 xontrib-sh-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3793 2021-03-19 16:21:17.000000 xontrib-sh-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-19 16:21:25.952780 xontrib-sh-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2021-03-19 16:21:17.000000 xontrib-sh-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-19 16:21:25.952780 xontrib-sh-0.3.0/xontrib/
--rw-r--r--   0 runner    (1001) docker     (121)     3456 2021-03-19 16:21:17.000000 xontrib-sh-0.3.0/xontrib/sh.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-19 16:21:25.952780 xontrib-sh-0.3.0/xontrib_sh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2021-03-19 16:21:25.000000 xontrib-sh-0.3.0/xontrib_sh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-03-19 16:21:25.000000 xontrib-sh-0.3.0/xontrib_sh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-19 16:21:25.000000 xontrib-sh-0.3.0/xontrib_sh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-03-19 16:21:25.000000 xontrib-sh-0.3.0/xontrib_sh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:20:59.067070 xontrib_sh-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-15 09:20:50.000000 xontrib_sh-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 09:20:50.000000 xontrib_sh-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-04-15 09:20:59.067070 xontrib_sh-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-15 09:20:50.000000 xontrib_sh-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:20:59.067070 xontrib_sh-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-15 09:20:50.000000 xontrib_sh-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:20:59.067070 xontrib_sh-0.3.1/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-15 09:20:50.000000 xontrib_sh-0.3.1/xontrib/sh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:20:59.067070 xontrib_sh-0.3.1/xontrib_sh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-04-15 09:20:59.000000 xontrib_sh-0.3.1/xontrib_sh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-15 09:20:59.000000 xontrib_sh-0.3.1/xontrib_sh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:20:59.000000 xontrib_sh-0.3.1/xontrib_sh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 09:20:59.000000 xontrib_sh-0.3.1/xontrib_sh.egg-info/top_level.txt
```

### Comparing `xontrib-sh-0.3.0/LICENSE` & `xontrib_sh-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xontrib-sh-0.3.0/README.md` & `xontrib_sh-0.3.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <p align="center">  
 Paste and run commands from bash, fish, zsh, tcsh in <a href="https://xon.sh">xonsh shell</a>.
 </p>
 
 <p align="center">  
-If you like the idea click ⭐ on the repo and stay tuned.
+If you like the idea click ⭐ on the repo and and <a href="https://twitter.com/intent/tweet?text=Nice%20xontrib%20for%20the%20xonsh%20shell!&url=https://github.com/anki-code/xontrib-sh" target="_blank">tweet</a>.
 </p>
 
 
 ## Install
 ```bash
 xpip install -U xontrib-sh
 echo 'xontrib load sh' >> ~/.xonshrc
@@ -38,15 +38,15 @@
 and this commands are environment agnostic and you want to run it without rewriting it on xonsh or run sh-shell. 
 
 For example you've found snippet of bash commands that check existing of `curl`:
 ```bash
 TMP=/tmp && cd $TMP && ( [[ -x $(command -v curl) ]] && echo "Yes" || echo "No" )  
 ```
 
-You hesitate how xonsh will execute this and you're absolutely right there will be syntax error. 
+You hesitate [how xonsh will execute this](https://github.com/anki-code/xonsh-cheatsheet/blob/main/README.md#three-most-frequent-things-that-newcomers-overlook) and you're absolutely right there will be syntax error. 
 To run this just start with `! ` or `!b ` or `!bash ` and paste the commands. As result you'll see the right message.
 
 ## Examples
 
 ### Bash brace expansion
 ```bash
 ! echo 01.{05..10}
@@ -112,9 +112,11 @@
 
 ## Additional options
 
 * `$XONTRIB_SH_USEFULL` (default `True`) - enables to set the shell explicitly by the name of the shell i.e. `!bash `.
 * `$XONTRIB_SH_USEFIRST` (default `True`) - enables to set the shell explicitly by the first letter i.e. `!b ` instead of `!bash `.
 
 ## Links 
+* This package is the part of [rc-awesome](https://github.com/anki-code/xontrib-rc-awesome) - awesome snippets of code for xonshrc in xonsh shell.
 * This package is the part of [ergopack](https://github.com/anki-code/xontrib-ergopack) - the pack of ergonomic xontribs.
 * This package was created with [xontrib cookiecutter template](https://github.com/xonsh/xontrib-cookiecutter).
+* [How to create a xonsh alias that have a behavior like in xontrib-sh?](https://github.com/anki-code/xontrib-sh/issues/6#issuecomment-1045978621)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
        Paste and run commands from bash, fish, zsh, tcsh in _x_o_n_s_h_ _s_h_e_l_l.
-          If you like the idea click â­ on the repo and stay tuned.
+           If you like the idea click â­ on the repo and and _t_w_e_e_t.
 ## Install ```bash xpip install -U xontrib-sh echo 'xontrib load sh' >>
 ~/.xonshrc # Reload xonsh ``` ## Usage Start the line with `! ` (exclamation
 mark with space) then paste the sh-compatible commands after it and run. The
 commands syntax will be tested in the shells from list (if installed) and the
 commands will be run in the first matching shell. By default list of shells
 contains bash and sh. The commands will be executed in the environment that
 will be inherited from current but if the commands modify the environment there
@@ -12,37 +12,43 @@
 ['bash', 'sh'] # default xontrib load sh ! echo hello ``` Also you can set the
 shell explicitly i.e. `!bash ` or `!b ` (the first letter of the shell). ## The
 main use case The main use case of `xontrib-sh` is when you copy and paste the
 sh-commands from some article or instruction and this commands are environment
 agnostic and you want to run it without rewriting it on xonsh or run sh-shell.
 For example you've found snippet of bash commands that check existing of
 `curl`: ```bash TMP=/tmp && cd $TMP && ( [[ -x $(command -v curl) ]] && echo
-"Yes" || echo "No" ) ``` You hesitate how xonsh will execute this and you're
-absolutely right there will be syntax error. To run this just start with `! `
-or `!b ` or `!bash ` and paste the commands. As result you'll see the right
-message. ## Examples ### Bash brace expansion ```bash ! echo 01.{05..10} # Or
-explicitly: !b echo 01.{05..10} !bash echo 01.{05..10} ``` ``` bash: 01.05
-01.06 01.07 01.08 01.09 01.10 ``` ### Multiline loop ```bash ! for i in 1 2 3
-do echo $i done ``` ``` bash: 1 2 3 ``` ### Use environment variables to pass
-values from xonsh to sh ```python $ENV = 'hello' ! echo $ENV! ``` ``` bash:
-hello! ``` ## Known issues #### Determining the shell on short command In case
-of usage many different shells the detection of the shell works perfect when
-the commands contain shell-specific syntax. But if you run the short command
-that could be valid in all shells the first matched shell will be chosen but
-it's could be wrong. For example you have bash and fish in the list of shells.
-The short fish command may be determined as bash command. As result the command
-will be failed: ```python $XONTRIB_SH_SHELLS = ['bash', 'fish'] xontrib load sh
-# Run fish command: ! set -U var1 value1 # bash: line 0: set: -U: invalid
-option ``` To avoid this use the explicit setting the shell i.e. `!fish set -
-U var1 value1`. Also, since __pwsh__ and __cmd__ shells don't have an option to
-detect their own syntax, they can only be invoked: - explicitly by their name,
-i.e. `!p ` or `!pwsh ` - implicitly via the `! ` prefix only when there is
-__one__ shell in `$XONTRIB_SH_SHELLS` #### Why it's better than [xonsh
-subprocess macros](https://xon.sh/tutorial_macros.html#subprocess-macros)?
-Xonsh subprocess macros is not supporting multiline commands and require more
-keystrokes. ## Additional options * `$XONTRIB_SH_USEFULL` (default `True`) -
-enables to set the shell explicitly by the name of the shell i.e. `!bash `. *
-`$XONTRIB_SH_USEFIRST` (default `True`) - enables to set the shell explicitly
-by the first letter i.e. `!b ` instead of `!bash `. ## Links * This package is
-the part of [ergopack](https://github.com/anki-code/xontrib-ergopack) - the
-pack of ergonomic xontribs. * This package was created with [xontrib
-cookiecutter template](https://github.com/xonsh/xontrib-cookiecutter).
+"Yes" || echo "No" ) ``` You hesitate [how xonsh will execute this](https://
+github.com/anki-code/xonsh-cheatsheet/blob/main/README.md#three-most-frequent-
+things-that-newcomers-overlook) and you're absolutely right there will be
+syntax error. To run this just start with `! ` or `!b ` or `!bash ` and paste
+the commands. As result you'll see the right message. ## Examples ### Bash
+brace expansion ```bash ! echo 01.{05..10} # Or explicitly: !b echo 01.{05..10}
+!bash echo 01.{05..10} ``` ``` bash: 01.05 01.06 01.07 01.08 01.09 01.10 ```
+### Multiline loop ```bash ! for i in 1 2 3 do echo $i done ``` ``` bash: 1 2 3
+``` ### Use environment variables to pass values from xonsh to sh ```python
+$ENV = 'hello' ! echo $ENV! ``` ``` bash: hello! ``` ## Known issues ####
+Determining the shell on short command In case of usage many different shells
+the detection of the shell works perfect when the commands contain shell-
+specific syntax. But if you run the short command that could be valid in all
+shells the first matched shell will be chosen but it's could be wrong. For
+example you have bash and fish in the list of shells. The short fish command
+may be determined as bash command. As result the command will be failed:
+```python $XONTRIB_SH_SHELLS = ['bash', 'fish'] xontrib load sh # Run fish
+command: ! set -U var1 value1 # bash: line 0: set: -U: invalid option ``` To
+avoid this use the explicit setting the shell i.e. `!fish set -U var1 value1`.
+Also, since __pwsh__ and __cmd__ shells don't have an option to detect their
+own syntax, they can only be invoked: - explicitly by their name, i.e. `!p ` or
+`!pwsh ` - implicitly via the `! ` prefix only when there is __one__ shell in
+`$XONTRIB_SH_SHELLS` #### Why it's better than [xonsh subprocess macros](https:
+//xon.sh/tutorial_macros.html#subprocess-macros)? Xonsh subprocess macros is
+not supporting multiline commands and require more keystrokes. ## Additional
+options * `$XONTRIB_SH_USEFULL` (default `True`) - enables to set the shell
+explicitly by the name of the shell i.e. `!bash `. * `$XONTRIB_SH_USEFIRST`
+(default `True`) - enables to set the shell explicitly by the first letter i.e.
+`!b ` instead of `!bash `. ## Links * This package is the part of [rc-awesome]
+(https://github.com/anki-code/xontrib-rc-awesome) - awesome snippets of code
+for xonshrc in xonsh shell. * This package is the part of [ergopack](https://
+github.com/anki-code/xontrib-ergopack) - the pack of ergonomic xontribs. * This
+package was created with [xontrib cookiecutter template](https://github.com/
+xonsh/xontrib-cookiecutter). * [How to create a xonsh alias that have a
+behavior like in xontrib-sh?](https://github.com/anki-code/xontrib-sh/issues/
+6#issuecomment-1045978621)
```

### Comparing `xontrib-sh-0.3.0/setup.py` & `xontrib_sh-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 except (IOError, OSError):
     long_description = ''
 
 setup(
     name='xontrib-sh',
-    version='0.3.0',
+    version='0.3.1',
     license='BSD',
     author='anki',
     author_email='author@example.com',
     description="Paste and run commands from bash, zsh, fish, tcsh, pwsh, cmd in xonsh shell.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
```

### Comparing `xontrib-sh-0.3.0/xontrib/sh.py` & `xontrib_sh-0.3.1/xontrib/sh.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,24 @@
+"""Paste and run commands from bash, zsh, fish, tcsh in xonsh shell. """
+
 from shutil import which
 
-_shells = list(__xonsh__.env.get('XONTRIB_SH_SHELLS', ['bash', 'sh']))
+def parse_shells_env(shells_env):
+    if isinstance(shells_env, str):
+        if '[' in shells_env: # string representation of a list
+            return shells_env.strip('[]').replace("'", "").split(',')
+        return [shells_env.replace("'", "")] #single shell
+    return list(shells_env)
+
+_shells = parse_shells_env(__xonsh__.env.get('XONTRIB_SH_SHELLS', ['bash', 'sh']))
 _bash_win = 'bash.exe'
 _installed_shells = []
 _match_first_char = __xonsh__.env.get('XONTRIB_SH_MATCHFIRST', True)
 _match_full_name = __xonsh__.env.get('XONTRIB_SH_MATCHFULL', True)
-_shells_without_syntax_check = ['pwsh', 'powershell', 'cmd']
-
+_shells_without_syntax_check = ['pwsh', 'powershell', 'cmd', 'nu']
 
 @events.on_transform_command
 def onepath(cmd, **kw):
     cmd_flag = '-c' # *sh flag to execute the specified commands, change to '/C' for cmd
 
     if len(cmd) > 2 and cmd.startswith('! '):
         if not _installed_shells:
```

