# Comparing `tmp/autofff-0.4.tar.gz` & `tmp/autofff-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofff-0.4.tar", max compression
+gzip compressed data, was "autofff-0.5.tar", max compression
```

## Comparing `autofff-0.4.tar` & `autofff-0.5.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1071 2021-11-25 22:24:10.348403 autofff-0.4/LICENSE
--rw-r--r--   0        0        0     9483 2021-11-25 22:24:10.348403 autofff-0.4/README.md
--rw-r--r--   0        0        0       78 2021-11-25 22:24:10.348403 autofff-0.4/autofff/__init__.py
--rw-r--r--   0        0        0     4613 2021-11-25 22:24:10.348403 autofff-0.4/autofff/__main__.py
--rw-r--r--   0        0        0     4244 2021-11-25 22:24:10.348403 autofff-0.4/autofff/config.py
--rw-r--r--   0        0        0     7844 2021-11-25 22:24:10.348403 autofff-0.4/autofff/generator.py
--rw-r--r--   0        0        0    12378 2021-11-25 22:24:10.348403 autofff-0.4/autofff/scanner.py
--rw-r--r--   0        0        0     4026 2021-11-25 22:24:10.348403 autofff-0.4/autofff/utils.py
--rw-r--r--   0        0        0     1056 2021-11-25 22:24:10.348403 autofff-0.4/pyproject.toml
--rw-r--r--   0        0        0    10593 2021-11-25 22:25:06.058524 autofff-0.4/setup.py
--rw-r--r--   0        0        0    10555 2021-11-25 22:25:06.059511 autofff-0.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-15 16:10:05.541621 autofff-0.5/LICENSE
+-rw-r--r--   0        0        0     9598 2024-04-15 16:10:05.541621 autofff-0.5/README.md
+-rw-r--r--   0        0        0       67 2024-04-15 16:10:05.541621 autofff-0.5/autofff/__init__.py
+-rw-r--r--   0        0        0     4613 2024-04-15 16:10:05.541621 autofff-0.5/autofff/__main__.py
+-rw-r--r--   0        0        0     4250 2024-04-15 16:10:05.541621 autofff-0.5/autofff/config.py
+-rw-r--r--   0        0        0     7950 2024-04-15 16:10:05.541621 autofff-0.5/autofff/generator.py
+-rw-r--r--   0        0        0    12462 2024-04-15 16:10:05.541621 autofff-0.5/autofff/scanner.py
+-rw-r--r--   0        0        0     4026 2024-04-15 16:10:05.541621 autofff-0.5/autofff/utils.py
+-rw-r--r--   0        0        0     1243 2024-04-15 16:10:05.545621 autofff-0.5/pyproject.toml
+-rw-r--r--   0        0        0    10960 1970-01-01 00:00:00.000000 autofff-0.5/PKG-INFO
```

### Comparing `autofff-0.4/LICENSE` & `autofff-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autofff-0.4/README.md` & `autofff-0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # AutoFFF
 
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ChiefGokhlayeh/autofff/master.svg)](https://results.pre-commit.ci/latest/github/ChiefGokhlayeh/autofff/master)
 [![build](https://github.com/ChiefGokhlayeh/autofff/actions/workflows/build.yml/badge.svg)](https://github.com/ChiefGokhlayeh/autofff/actions/workflows/build.yml)
 [![PyPI version](https://badge.fury.io/py/autofff.svg)](https://badge.fury.io/py/autofff)
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 Auto-generate [FFF](https://github.com/meekrosoft/fff) fake definitions for C API header files.
 
 Incorporate this script into your normal build environment (like _make_) and automatically generate test-headers with faked function definitions ready-to-use with [FFF](https://github.com/meekrosoft/fff)'s own _gtest_ or some other unit-testing-framework.
@@ -84,22 +85,22 @@
 ### As a Python Package
 
 ```python
 import autofff
 
 import os.path
 
-targetHeader = input("Enter the path of the header you would like to scan: ")
-outputHeader = input("Enter the path of the target header file which shall be generated: ")
+targetHeader = "examples/simple-headers/driver.h"
+outputHeader = "output/driver_th.h"
 fakes = './autofff/dependencies/pycparser/utils/fake_libc_include'
 
-scnr = autofff.GCCScanner(targetHeader, fakes) # Create GCC code scanner
+scnr = autofff.scanner.GCCScanner(targetHeader, fakes) # Create GCC code scanner
 result = scnr.scan() # Scan for function declarations and definitions
 
-gen = autofff.SimpleFakeGenerator(os.path.splitext(os.path.basename(outputHeader))[0], targetHeader) # Create new generator with name output-header and path to target-header
+gen = autofff.generator.SimpleFakeGenerator(os.path.splitext(os.path.basename(outputHeader))[0], targetHeader) # Create new generator with name output-header and path to target-header
 
 if not os.path.exists(os.path.dirname(outputHeader)):
     dirname = os.path.dirname(outputHeader)
     os.makedirs(dirname)
 
 with open(outputHeader, "w") as fs:
     gen.generate(result, fs) # Generate fff-fakes from scanner-result
@@ -110,15 +111,15 @@
 The format of the generated test-header obviously depends on the specifics of the `FakeGenerator` being used.
 
 1. The `BareFakeGenerator` will only generate the `FAKE_VALUE_`- and `FAKE_VOID_FUNC` macros without any decorations, like include guards or header includes. Use this generator if you want to add your own (shell-based-)processing on top.
 2. The `SimpleFakeGenerator` will generate a "minimum viable test header", meaning the result should be compilable without too much effort.
 
 ### In-Header Defined Functions
 
-In some API headers functions may be defined within the header. This will cause issues when trying to fake this function, because by including the header the function definition is copied into each translation unit. If we try to apply a fake definition the usual way, we will end up with a _"redefinition of function *x*"_ error.
+In some API headers functions may be defined within the header. This will cause issues when trying to fake this function, because by including the header the function definition is copied into each translation unit. If we try to apply a fake definition the usual way, we will end up with a _"redefinition of function **x**"_ error.
 
 _AutoFFF_ implements a workaround to avoid this redefinition error and allowing to fake the original function. This workaround simply consists of some defines which will re-route any call to the original in-header definition to our faked one. For this to work it is required that the test-header is included (and thereby pre-processed) _before_ any function call to the function under consideration is instructed, i.e. the test-header must be included _before_ the CuT. Any function call that is processed before the workaround is being pre-processed will leave this function call targeted towards the original in-header definition.
 
 In practice the workaround looks like this:
 
 ```c
 /* api.h */
```

### Comparing `autofff-0.4/autofff/__main__.py` & `autofff-0.5/autofff/__main__.py`

 * *Files identical despite different names*

### Comparing `autofff-0.4/autofff/config.py` & `autofff-0.5/autofff/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,15 @@
 GCC_SCANNER_CPP_INCLUDE_FILE_PREFIX = "cpp_include_file_prefix"
 GCC_SCANNER_CPP_INCLUDE_FILE_PREFIX_DEF = "-include"
 
 GCC_SCANNER_CPP_DEFINE_PREFIX = "cpp_define_prefix"
 GCC_SCANNER_CPP_DEFINE_PREFIX_DEF = "-D"
 
 GCC_SCANNER_NON_STANDARD_IGNORE_PATTERN = "non_standard_ignore_pattern"
-GCC_SCANNER_NON_STANDARD_IGNORE_PATTERN_DEF = (
-    r"([\s\n]*(__asm|asm)[\s\n]*(volatile|[\s\n]*)(goto|[\s\n]*)(.|\n|;)*?;)"
-)
+GCC_SCANNER_NON_STANDARD_IGNORE_PATTERN_DEF = r"([\s\n]*(\W(__asm|asm|__asm__)\W)[\s\n]*(volatile|[\s\n]*)(goto|[\s\n]*)(.|\n|;)*?;)"
 
 GCC_SCANNER_ERROR_CONTEXT_PREV_LINES = "error_context_prev_lines"
 GCC_SCANNER_ERROR_CONTEXT_PREV_LINES_MIN = 0
 GCC_SCANNER_ERROR_CONTEXT_PREV_LINES_DEF = 5
 GCC_SCANNER_ERROR_CONTEXT_POST_LINES = "error_context_post_lines"
 GCC_SCANNER_ERROR_CONTEXT_POST_LINES_MIN = 0
 GCC_SCANNER_ERROR_CONTEXT_POST_LINES_DEF = 5
```

### Comparing `autofff-0.4/autofff/generator.py` & `autofff-0.5/autofff/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,18 @@
     def _generateTypeDefForDecl(self, decl: Decl) -> str:
         typedefs = ""
         for param in filter(
             lambda p: utils.is_function_pointer_type(p.type), decl.type.args.params
         ):
             name = utils.create_typedef_name_for_fnc_ptr(decl, param)
 
-            param.type.type.type.declname = name
+            type = param.type.type.type
+            while not hasattr(type, "declname"):
+                type = type.type
+            type.declname = name
             typedef = Typedef(name, param.quals, ["typedef"], param.type)
 
             param.type = TypeDecl(
                 param.name, param.type.quals, None, IdentifierType([name])
             )
             typedefs += f"{self.cGen.visit_Typedef(typedef)};\n"
         return typedefs
```

### Comparing `autofff-0.4/autofff/scanner.py` & `autofff-0.5/autofff/scanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,17 @@
         ignorePattern: str = None,
     ) -> None:
         self.inputFile = inputFile
         self.fakes = fakes
         self.includes = includes
         self.includeFiles = includeFiles
         self.defines = defines
-        if isinstance(ignorePattern, str):
+        if ignorePattern is None:
+            self.ignorePattern = re.compile("")
+        elif isinstance(ignorePattern, str):
             self.ignorePattern = re.compile(ignorePattern)
         else:
             self.ignorePattern = ignorePattern
 
     def scan(self) -> ScannerResult:
         ast = self._call_parse(self.inputFile)
         return ScannerResult(
```

### Comparing `autofff-0.4/autofff/utils.py` & `autofff-0.5/autofff/utils.py`

 * *Files identical despite different names*

### Comparing `autofff-0.4/pyproject.toml` & `autofff-0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 [tool.poetry]
 name = "autofff"
-version = "0.4"
+version = "0.5"
 description = "Auto-generate FFF fake definitions for C API header files"
 authors = ["Andreas Baulig <free.geronimo@hotmail.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ChiefGokhlayeh/autofff"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: C",
     "Programming Language :: C++",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.6",
     "Topic :: Software Development :: Code Generators",
     "Topic :: Software Development :: Testing",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 pycparser = "^2.21"
-overrides = "^6.1.0"
-configobj = "^5.0.6"
+overrides = ">=6.5,<8.0"
+configobj = "^5.0.8"
 validator = "^0.7.1"
+phmutest = "^0.0.3"
 
 [tool.poetry.dev-dependencies]
-black = "^21.11b1"
-rope = "^0.22.0"
-flake8 = "^4.0.1"
-pre-commit = "^2.15.0"
+black = "^24.4.0"
+flake8 = "^7.0.0"
+pre-commit = "^3.7.0"
 
 [tool.poetry.scripts]
 autofff = "autofff.__main__:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autofff-0.4/PKG-INFO` & `autofff-0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 Metadata-Version: 2.1
 Name: autofff
-Version: 0.4
+Version: 0.5
 Summary: Auto-generate FFF fake definitions for C API header files
 Home-page: https://github.com/ChiefGokhlayeh/autofff
 License: MIT
 Author: Andreas Baulig
 Author-email: free.geronimo@hotmail.de
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: configobj (>=5.0.6,<6.0.0)
-Requires-Dist: overrides (>=6.1.0,<7.0.0)
+Requires-Dist: configobj (>=5.0.8,<6.0.0)
+Requires-Dist: overrides (>=6.5,<8.0)
+Requires-Dist: phmutest (>=0.0.3,<0.0.4)
 Requires-Dist: pycparser (>=2.21,<3.0)
 Requires-Dist: validator (>=0.7.1,<0.8.0)
 Project-URL: Repository, https://github.com/ChiefGokhlayeh/autofff
 Description-Content-Type: text/markdown
 
 # AutoFFF
 
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ChiefGokhlayeh/autofff/master.svg)](https://results.pre-commit.ci/latest/github/ChiefGokhlayeh/autofff/master)
 [![build](https://github.com/ChiefGokhlayeh/autofff/actions/workflows/build.yml/badge.svg)](https://github.com/ChiefGokhlayeh/autofff/actions/workflows/build.yml)
 [![PyPI version](https://badge.fury.io/py/autofff.svg)](https://badge.fury.io/py/autofff)
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 Auto-generate [FFF](https://github.com/meekrosoft/fff) fake definitions for C API header files.
 
 Incorporate this script into your normal build environment (like _make_) and automatically generate test-headers with faked function definitions ready-to-use with [FFF](https://github.com/meekrosoft/fff)'s own _gtest_ or some other unit-testing-framework.
@@ -111,22 +118,22 @@
 ### As a Python Package
 
 ```python
 import autofff
 
 import os.path
 
-targetHeader = input("Enter the path of the header you would like to scan: ")
-outputHeader = input("Enter the path of the target header file which shall be generated: ")
+targetHeader = "examples/simple-headers/driver.h"
+outputHeader = "output/driver_th.h"
 fakes = './autofff/dependencies/pycparser/utils/fake_libc_include'
 
-scnr = autofff.GCCScanner(targetHeader, fakes) # Create GCC code scanner
+scnr = autofff.scanner.GCCScanner(targetHeader, fakes) # Create GCC code scanner
 result = scnr.scan() # Scan for function declarations and definitions
 
-gen = autofff.SimpleFakeGenerator(os.path.splitext(os.path.basename(outputHeader))[0], targetHeader) # Create new generator with name output-header and path to target-header
+gen = autofff.generator.SimpleFakeGenerator(os.path.splitext(os.path.basename(outputHeader))[0], targetHeader) # Create new generator with name output-header and path to target-header
 
 if not os.path.exists(os.path.dirname(outputHeader)):
     dirname = os.path.dirname(outputHeader)
     os.makedirs(dirname)
 
 with open(outputHeader, "w") as fs:
     gen.generate(result, fs) # Generate fff-fakes from scanner-result
@@ -137,15 +144,15 @@
 The format of the generated test-header obviously depends on the specifics of the `FakeGenerator` being used.
 
 1. The `BareFakeGenerator` will only generate the `FAKE_VALUE_`- and `FAKE_VOID_FUNC` macros without any decorations, like include guards or header includes. Use this generator if you want to add your own (shell-based-)processing on top.
 2. The `SimpleFakeGenerator` will generate a "minimum viable test header", meaning the result should be compilable without too much effort.
 
 ### In-Header Defined Functions
 
-In some API headers functions may be defined within the header. This will cause issues when trying to fake this function, because by including the header the function definition is copied into each translation unit. If we try to apply a fake definition the usual way, we will end up with a _"redefinition of function *x*"_ error.
+In some API headers functions may be defined within the header. This will cause issues when trying to fake this function, because by including the header the function definition is copied into each translation unit. If we try to apply a fake definition the usual way, we will end up with a _"redefinition of function **x**"_ error.
 
 _AutoFFF_ implements a workaround to avoid this redefinition error and allowing to fake the original function. This workaround simply consists of some defines which will re-route any call to the original in-header definition to our faked one. For this to work it is required that the test-header is included (and thereby pre-processed) _before_ any function call to the function under consideration is instructed, i.e. the test-header must be included _before_ the CuT. Any function call that is processed before the workaround is being pre-processed will leave this function call targeted towards the original in-header definition.
 
 In practice the workaround looks like this:
 
 ```c
 /* api.h */
```

