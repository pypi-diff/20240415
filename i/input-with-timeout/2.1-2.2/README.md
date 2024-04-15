# Comparing `tmp/input-with-timeout-2.1.tar.gz` & `tmp/input_with_timeout-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "input-with-timeout-2.1.tar", last modified: Sun Mar 31 22:12:04 2024, max compression
+gzip compressed data, was "input_with_timeout-2.2.tar", last modified: Mon Apr 15 07:05:22 2024, max compression
```

## Comparing `input-with-timeout-2.1.tar` & `input_with_timeout-2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 22:12:04.695344 input-with-timeout-2.1/
--rw-rw-rw-   0        0        0     1086 2024-03-25 00:08:57.000000 input-with-timeout-2.1/LICENSE
--rw-rw-rw-   0        0        0     1829 2024-03-31 22:12:04.695344 input-with-timeout-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1099 2024-03-31 21:57:30.000000 input-with-timeout-2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 22:12:04.676346 input-with-timeout-2.1/input_with_timeout/
--rw-rw-rw-   0        0        0     1148 2024-03-31 21:55:52.000000 input-with-timeout-2.1/input_with_timeout/__init__.py
--rw-rw-rw-   0        0        0      840 2024-03-31 22:10:46.000000 input-with-timeout-2.1/input_with_timeout/__version__.py
--rw-rw-rw-   0        0        0      502 2024-03-29 23:03:45.000000 input-with-timeout-2.1/input_with_timeout/console_output.py
--rw-rw-rw-   0        0        0     4287 2024-03-31 22:10:23.000000 input-with-timeout-2.1/input_with_timeout/main.py
-drwxrwxrwx   0        0        0        0 2024-03-31 22:12:04.694345 input-with-timeout-2.1/input_with_timeout.egg-info/
--rw-rw-rw-   0        0        0     1829 2024-03-31 22:12:04.000000 input-with-timeout-2.1/input_with_timeout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2024-03-31 22:12:04.000000 input-with-timeout-2.1/input_with_timeout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 22:12:04.000000 input-with-timeout-2.1/input_with_timeout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-03-31 22:12:04.000000 input-with-timeout-2.1/input_with_timeout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-31 22:12:04.703346 input-with-timeout-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1229 2024-03-31 22:00:32.000000 input-with-timeout-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:05:22.834160 input_with_timeout-2.2/
+-rw-rw-rw-   0        0        0     1086 2024-03-25 00:08:57.000000 input_with_timeout-2.2/LICENSE
+-rw-rw-rw-   0        0        0     1830 2024-04-15 07:05:22.834160 input_with_timeout-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1100 2024-04-11 07:44:55.000000 input_with_timeout-2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 07:05:22.822158 input_with_timeout-2.2/input_with_timeout/
+-rw-rw-rw-   0        0        0     1148 2024-03-31 21:55:52.000000 input_with_timeout-2.2/input_with_timeout/__init__.py
+-rw-rw-rw-   0        0        0      840 2024-04-15 06:53:41.000000 input_with_timeout-2.2/input_with_timeout/__version__.py
+-rw-rw-rw-   0        0        0      435 2024-04-15 06:51:11.000000 input_with_timeout-2.2/input_with_timeout/console_output.py
+-rw-rw-rw-   0        0        0     4362 2024-04-15 06:53:07.000000 input_with_timeout-2.2/input_with_timeout/main.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:05:22.833158 input_with_timeout-2.2/input_with_timeout.egg-info/
+-rw-rw-rw-   0        0        0     1830 2024-04-15 07:05:22.000000 input_with_timeout-2.2/input_with_timeout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-15 07:05:22.000000 input_with_timeout-2.2/input_with_timeout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 07:05:22.000000 input_with_timeout-2.2/input_with_timeout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-15 07:05:22.000000 input_with_timeout-2.2/input_with_timeout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 07:05:22.834160 input_with_timeout-2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2024-03-31 22:00:32.000000 input_with_timeout-2.2/setup.py
```

### Comparing `input-with-timeout-2.1/LICENSE` & `input_with_timeout-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `input-with-timeout-2.1/PKG-INFO` & `input_with_timeout-2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: input-with-timeout
-Version: 2.1
+Version: 2.2
 Summary: The 'input-with-timeout' module provides a cross-platform method to capture user input with a timeout feature.
 Home-page: http://github.com/mamahoos/input_with_timeout
 Author: mamahoos
 Author-email: m4m4hoos@gmail.com
 License: MIT License
 Keywords: python,cross-platform,stdout,stin,console
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 This Python project provides a function `input_with_timeout` which allows capturing user input with a specified `timeout`. If the user does not provide input within the `timeout` period, a `TimeoutError` is raised.
 
 ## Installation
 You can install this packag using the following commands:
 ```bash
 pip install input-with-timeout
 ```
-or
+ or
 ```bash
 pip install git+https://github.com/mamahoos/python-input-with-timeout
 ```
 
 ## Features
 
 - Customizable `timeout` for user input.
```

### Comparing `input-with-timeout-2.1/README.md` & `input_with_timeout-2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This Python project provides a function `input_with_timeout` which allows capturing user input with a specified `timeout`. If the user does not provide input within the `timeout` period, a `TimeoutError` is raised.
 
 ## Installation
 You can install this packag using the following commands:
 ```bash
 pip install input-with-timeout
 ```
-or
+ or
 ```bash
 pip install git+https://github.com/mamahoos/python-input-with-timeout
 ```
 
 ## Features
 
 - Customizable `timeout` for user input.
```

### Comparing `input-with-timeout-2.1/input_with_timeout/__init__.py` & `input_with_timeout-2.2/input_with_timeout/__init__.py`

 * *Files identical despite different names*

### Comparing `input-with-timeout-2.1/input_with_timeout/__version__.py` & `input_with_timeout-2.2/input_with_timeout/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __title__        = 'input-with-timeout'
 __description__  = 'The \'input-with-timeout\' module provides a cross-platform method to capture user input with a timeout feature.'
-__version__      = '2.1'
-__version_info__ = (2,1)
+__version__      = '2.2'
+__version_info__ = (2,2)
 __author__       = 'mamahoos'
 __author_email__ = 'm4m4hoos@gmail.com'
 __url__          = 'http://github.com/mamahoos/input_with_timeout'
 __copyright__    = 'Copyright (c) 2024 mamahoos'
 __license__      = 'MIT License'
 __keywords__     = ['input', 'timeout', 'user input', 'cross-platform']
 __platforms__    = 'Any'
```

### Comparing `input-with-timeout-2.1/input_with_timeout/main.py` & `input_with_timeout-2.2/input_with_timeout/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from .console_output import cout, endl
-from typing import Union, Any
-import builtins
+import builtins, types, typing
 
 
 
 def windows_input_with_timeout(prompt, timeout):
     cout << prompt              # Print the prompt to the console
 
     CR = chr(0x0D)              # Carriage return character
     LF = chr(0x0A)              # Line feed character 
     BS = chr(0x08)              # Backspace character
     SP = chr(0x20)              # Space character 
+    ET = chr(0x03)              # End of text character
 
     DELAY = 5e-2                # 50 ms
     line  = ''                  # Initialize an empty line buffer
     start = time.monotonic()
     end   = start + timeout     # Calculate the end time for the timeout
 
     while (time.monotonic() < end):
         if msvcrt.kbhit():              # If a key has been pressed
-            ch = msvcrt.getch() \
-            .decode(encoding='utf-8')   # Get the pressed character and decode it to utf-8
+            ch = msvcrt.getwch()   # Get the pressed character
                         
             if ch in (CR, LF):          # If the character is a carriage return or line feed
                 cout << endl            # cout << CR << LF
                 return line
             
+            elif ch == ET:              # Handling Ctrl+C
+                raise KeyboardInterrupt
+
             elif ch == BS:              # Handle backspace character
                 if line:                # If the line is not empty 
                     line = line[:-1]    # Remove the last character from the line
                     cout << BS << SP    # Clear the last character from the screen
                     cout << BS          # Move the cursor back
 
             else:
@@ -58,15 +60,15 @@
         else:
             raise TimeoutError("Timeout occurred.")
     finally:
         termios.tcsetattr(sys.stdin, termios.TCSADRAIN, settings)
 
 
 
-def input_with_timeout(prompt: Any = '', /, timeout: Union[int, float, None] = 20.0) -> str:
+def input_with_timeout(prompt: typing.Any = '', /, timeout: typing.Union[int, float, None] = 20.0) -> str:
     """\
     This function prompts the user for input and returns the input if received within the specified `timeout`.
     If the input is not received within the `timeout`, a TimeoutError is raised.
 
     ### Parameters:
     - prompt (Any): The text to display before waiting for input.
     - timeout (Union[int, float, None]): The maximum time to wait for input. Set to `None` for no `timeout`.
@@ -84,15 +86,15 @@
         # To get input with a timeout:
         result = input_with_timeout("Please enter your input: ", timeout=15.0)
 
         # To get input without a timeout:
         result = input_with_timeout("Please enter your input: ", timeout=None)
     """
 
-    if not (isinstance(timeout, (int, float)) or timeout is None):
+    if not isinstance(timeout, (int, float, types.NoneType)):
         raise TypeError(f"timeout must be 'int' or 'float' or 'None', not {type(timeout)}.")
     elif timeout is None:
         return builtins.input(prompt)
     elif timeout <= 0:
         raise ValueError(f"timeout value must be greater than zero, timeout: {timeout}.")
 
     try:
@@ -101,9 +103,9 @@
         func = windows_input_with_timeout
     
     except ImportError:
         global sys, tty, termios, select
         import sys, tty, termios, select
         func = unix_input_with_timeout
 
-    finally:
-        return func(prompt, timeout)
+    return func(prompt, timeout)
+
```

### Comparing `input-with-timeout-2.1/input_with_timeout.egg-info/PKG-INFO` & `input_with_timeout-2.2/input_with_timeout.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: input-with-timeout
-Version: 2.1
+Version: 2.2
 Summary: The 'input-with-timeout' module provides a cross-platform method to capture user input with a timeout feature.
 Home-page: http://github.com/mamahoos/input_with_timeout
 Author: mamahoos
 Author-email: m4m4hoos@gmail.com
 License: MIT License
 Keywords: python,cross-platform,stdout,stin,console
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 This Python project provides a function `input_with_timeout` which allows capturing user input with a specified `timeout`. If the user does not provide input within the `timeout` period, a `TimeoutError` is raised.
 
 ## Installation
 You can install this packag using the following commands:
 ```bash
 pip install input-with-timeout
 ```
-or
+ or
 ```bash
 pip install git+https://github.com/mamahoos/python-input-with-timeout
 ```
 
 ## Features
 
 - Customizable `timeout` for user input.
```

### Comparing `input-with-timeout-2.1/setup.py` & `input_with_timeout-2.2/setup.py`

 * *Files identical despite different names*

