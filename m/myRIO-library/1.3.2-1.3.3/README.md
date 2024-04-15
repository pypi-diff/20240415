# Comparing `tmp/myRIO_library-1.3.2.tar.gz` & `tmp/myrio_library-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myRIO_library-1.3.2.tar", last modified: Fri Apr 12 15:52:45 2024, max compression
+gzip compressed data, was "myrio_library-1.3.3.tar", last modified: Mon Apr 15 08:35:37 2024, max compression
```

## Comparing `myRIO_library-1.3.2.tar` & `myrio_library-1.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 15:52:45.419149 myRIO_library-1.3.2/
--rw-rw-rw-   0        0        0     3283 2024-04-12 15:52:45.413170 myRIO_library-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2249 2024-03-14 22:01:02.000000 myRIO_library-1.3.2/README.md
--rw-rw-rw-   0        0        0       78 2024-03-01 11:10:42.000000 myRIO_library-1.3.2/pyproject.toml
--rw-rw-rw-   0        0        0     1273 2024-04-12 15:52:45.439090 myRIO_library-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      969 2024-04-12 15:41:40.000000 myRIO_library-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:52:44.301413 myRIO_library-1.3.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 15:52:44.551957 myRIO_library-1.3.2/src/myRIO_API/
--rw-rw-rw-   0        0        0       73 2024-03-11 14:39:40.000000 myRIO_library-1.3.2/src/myRIO_API/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:52:44.582806 myRIO_library-1.3.2/src/myRIO_API/examples/
--rw-rw-rw-   0        0        0     1067 2024-03-11 16:34:21.000000 myRIO_library-1.3.2/src/myRIO_API/examples/README_server.txt
--rw-rw-rw-   0        0        0      602 2024-03-11 14:24:10.000000 myRIO_library-1.3.2/src/myRIO_API/examples/myRIO_API
--rw-rw-rw-   0        0        0     6337 2024-04-12 15:12:08.000000 myRIO_library-1.3.2/src/myRIO_API/myRIO_API.py
--rw-rw-rw-   0        0        0     1202 2024-04-12 15:41:25.000000 myRIO_library-1.3.2/src/myRIO_API/version.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:52:44.698709 myRIO_library-1.3.2/src/myRIO_API_client/
--rw-rw-rw-   0        0        0       80 2024-03-12 05:47:26.000000 myRIO_library-1.3.2/src/myRIO_API_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:52:44.719778 myRIO_library-1.3.2/src/myRIO_API_client/examples/
--rw-rw-rw-   0        0        0      612 2024-03-12 09:54:55.000000 myRIO_library-1.3.2/src/myRIO_API_client/examples/README_client.txt
--rw-rw-rw-   0        0        0     1955 2024-04-12 15:48:23.000000 myRIO_library-1.3.2/src/myRIO_API_client/examples/client_examples.py
--rw-rw-rw-   0        0        0     8147 2024-04-12 15:40:13.000000 myRIO_library-1.3.2/src/myRIO_API_client/myRIO_API_client.py
--rw-rw-rw-   0        0        0     1202 2024-04-12 15:41:17.000000 myRIO_library-1.3.2/src/myRIO_API_client/version.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:52:44.767102 myRIO_library-1.3.2/src/myRIO_base/
--rw-rw-rw-   0        0        0       74 2024-03-12 09:59:59.000000 myRIO_library-1.3.2/src/myRIO_base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:52:44.949242 myRIO_library-1.3.2/src/myRIO_base/data/
--rw-rw-rw-   0        0        0  2957199 2016-12-02 19:23:24.000000 myRIO_library-1.3.2/src/myRIO_base/data/Default.lvbitx
--rw-rw-rw-   0        0        0  2906853 2022-07-10 07:27:56.000000 myRIO_library-1.3.2/src/myRIO_base/data/High-throughput.lvbitx
-drwxrwxrwx   0        0        0        0 2024-04-12 15:52:45.234468 myRIO_library-1.3.2/src/myRIO_base/examples/
--rw-rw-rw-   0        0        0     2453 2024-04-12 14:42:07.000000 myRIO_library-1.3.2/src/myRIO_base/examples/PWM_tests.py
--rw-rw-rw-   0        0        0   211136 2024-04-10 08:32:38.000000 myRIO_library-1.3.2/src/myRIO_base/examples/PacManDeath.csv
--rw-rw-rw-   0        0        0     1755 2024-04-12 14:42:41.000000 myRIO_library-1.3.2/src/myRIO_base/examples/analog-inputs-and-outputs.py
--rw-rw-rw-   0        0        0     2625 2024-04-12 14:42:45.000000 myRIO_library-1.3.2/src/myRIO_base/examples/digital-inputs-and-outputs.py
--rw-rw-rw-   0        0        0     1434 2024-04-12 14:42:18.000000 myRIO_library-1.3.2/src/myRIO_base/examples/mxp-board-tests.py
--rw-rw-rw-   0        0        0      708 2024-04-10 08:53:54.000000 myRIO_library-1.3.2/src/myRIO_base/examples/waveform-test.py
--rw-rw-rw-   0        0        0    27024 2024-04-12 14:31:51.000000 myRIO_library-1.3.2/src/myRIO_base/myRIO_base.py
--rw-rw-rw-   0        0        0     1202 2024-04-12 15:41:08.000000 myRIO_library-1.3.2/src/myRIO_base/version.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:52:45.403373 myRIO_library-1.3.2/src/myRIO_library.egg-info/
--rw-rw-rw-   0        0        0     3283 2024-04-12 15:52:44.000000 myRIO_library-1.3.2/src/myRIO_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1030 2024-04-12 15:52:44.000000 myRIO_library-1.3.2/src/myRIO_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 15:52:44.000000 myRIO_library-1.3.2/src/myRIO_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      156 2024-04-12 15:52:44.000000 myRIO_library-1.3.2/src/myRIO_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2024-04-12 15:52:44.000000 myRIO_library-1.3.2/src/myRIO_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 08:35:37.518160 myrio_library-1.3.3/
+-rw-rw-rw-   0        0        0     3283 2024-04-15 08:35:37.514164 myrio_library-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2249 2024-03-14 22:01:02.000000 myrio_library-1.3.3/README.md
+-rw-rw-rw-   0        0        0       78 2024-03-01 11:10:42.000000 myrio_library-1.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1273 2024-04-15 08:35:37.520142 myrio_library-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      969 2024-04-15 08:35:23.000000 myrio_library-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:35:37.317151 myrio_library-1.3.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 08:35:37.351150 myrio_library-1.3.3/src/myRIO_API/
+-rw-rw-rw-   0        0        0       73 2024-03-11 14:39:40.000000 myrio_library-1.3.3/src/myRIO_API/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:35:37.361183 myrio_library-1.3.3/src/myRIO_API/examples/
+-rw-rw-rw-   0        0        0     1067 2024-03-11 16:34:21.000000 myrio_library-1.3.3/src/myRIO_API/examples/README_server.txt
+-rw-rw-rw-   0        0        0      602 2024-03-11 14:24:10.000000 myrio_library-1.3.3/src/myRIO_API/examples/myRIO_API
+-rw-rw-rw-   0        0        0     6337 2024-04-12 15:12:08.000000 myrio_library-1.3.3/src/myRIO_API/myRIO_API.py
+-rw-rw-rw-   0        0        0     1243 2024-04-15 08:33:34.000000 myrio_library-1.3.3/src/myRIO_API/version.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:35:37.375188 myrio_library-1.3.3/src/myRIO_API_client/
+-rw-rw-rw-   0        0        0       80 2024-03-12 05:47:26.000000 myrio_library-1.3.3/src/myRIO_API_client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:35:37.390151 myrio_library-1.3.3/src/myRIO_API_client/examples/
+-rw-rw-rw-   0        0        0      612 2024-03-12 09:54:55.000000 myrio_library-1.3.3/src/myRIO_API_client/examples/README_client.txt
+-rw-rw-rw-   0        0        0     1955 2024-04-12 15:48:23.000000 myrio_library-1.3.3/src/myRIO_API_client/examples/client_examples.py
+-rw-rw-rw-   0        0        0     8147 2024-04-12 15:40:13.000000 myrio_library-1.3.3/src/myRIO_API_client/myRIO_API_client.py
+-rw-rw-rw-   0        0        0     1243 2024-04-15 08:33:27.000000 myrio_library-1.3.3/src/myRIO_API_client/version.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:35:37.413175 myrio_library-1.3.3/src/myRIO_base/
+-rw-rw-rw-   0        0        0       74 2024-03-12 09:59:59.000000 myrio_library-1.3.3/src/myRIO_base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:35:37.429146 myrio_library-1.3.3/src/myRIO_base/data/
+-rw-rw-rw-   0        0        0  2957199 2016-12-02 19:23:24.000000 myrio_library-1.3.3/src/myRIO_base/data/Default.lvbitx
+-rw-rw-rw-   0        0        0  2906853 2022-07-10 07:27:56.000000 myrio_library-1.3.3/src/myRIO_base/data/High-throughput.lvbitx
+drwxrwxrwx   0        0        0        0 2024-04-15 08:35:37.480147 myrio_library-1.3.3/src/myRIO_base/examples/
+-rw-rw-rw-   0        0        0     2453 2024-04-12 14:42:07.000000 myrio_library-1.3.3/src/myRIO_base/examples/PWM_tests.py
+-rw-rw-rw-   0        0        0   211136 2024-04-10 08:32:38.000000 myrio_library-1.3.3/src/myRIO_base/examples/PacManDeath.csv
+-rw-rw-rw-   0        0        0     1755 2024-04-12 14:42:41.000000 myrio_library-1.3.3/src/myRIO_base/examples/analog-inputs-and-outputs.py
+-rw-rw-rw-   0        0        0     2625 2024-04-12 14:42:45.000000 myrio_library-1.3.3/src/myRIO_base/examples/digital-inputs-and-outputs.py
+-rw-rw-rw-   0        0        0     1434 2024-04-12 14:42:18.000000 myrio_library-1.3.3/src/myRIO_base/examples/mxp-board-tests.py
+-rw-rw-rw-   0        0        0      708 2024-04-10 08:53:54.000000 myrio_library-1.3.3/src/myRIO_base/examples/waveform-test.py
+-rw-rw-rw-   0        0        0    27093 2024-04-15 08:32:19.000000 myrio_library-1.3.3/src/myRIO_base/myRIO_base.py
+-rw-rw-rw-   0        0        0     1243 2024-04-15 08:33:06.000000 myrio_library-1.3.3/src/myRIO_base/version.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:35:37.509145 myrio_library-1.3.3/src/myRIO_library.egg-info/
+-rw-rw-rw-   0        0        0     3283 2024-04-15 08:35:37.000000 myrio_library-1.3.3/src/myRIO_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1030 2024-04-15 08:35:37.000000 myrio_library-1.3.3/src/myRIO_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 08:35:37.000000 myrio_library-1.3.3/src/myRIO_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      156 2024-04-15 08:35:37.000000 myrio_library-1.3.3/src/myRIO_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2024-04-15 08:35:37.000000 myrio_library-1.3.3/src/myRIO_library.egg-info/top_level.txt
```

### Comparing `myRIO_library-1.3.2/PKG-INFO` & `myrio_library-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myRIO_library
-Version: 1.3.2
+Version: 1.3.3
 Summary: A library to control the myRIO board from National Instruments
 Home-page: https://github.com/AitzolEzeizaUPVEHU/myRIO_library
 Download-URL: https://github.com/AitzolEzeizaUPVEHU/myRIO_library/archive/refs/heads/main.zip
 Author: Aitzol Ezeiza Ramos
 Author-email: aitzol.ezeiza@ehu.eus
 License: MIT
 Keywords: myRIO,NI,National Instruments,LabVIEW,Python,FPGA,Real-Time,Embedded Systems
```

### Comparing `myRIO_library-1.3.2/README.md` & `myrio_library-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/setup.cfg` & `myrio_library-1.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/setup.py` & `myrio_library-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='myRIO_library',
-version='1.3.2',
+version='1.3.3',
 author='Aitzol Ezeiza Ramos',
 author_email='aitzol.ezeiza@ehu.eus',
 description='A library to control the myRIO board from National Instruments',
 long_description=long_description,
 long_description_content_type='text/markdown',
 
 packages=find_packages('src'),
```

### Comparing `myRIO_library-1.3.2/src/myRIO_API/examples/README_server.txt` & `myrio_library-1.3.3/src/myRIO_API/examples/README_server.txt`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/src/myRIO_API/examples/myRIO_API` & `myrio_library-1.3.3/src/myRIO_API/examples/myRIO_API`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/src/myRIO_API/myRIO_API.py` & `myrio_library-1.3.3/src/myRIO_API/myRIO_API.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/src/myRIO_API/version.py` & `myrio_library-1.3.3/src/myRIO_API/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # version.py
-__version__ = "1.3.2"
+__version__ = "1.3.3"
 
 """ version notes
 0.2.0: added __del__ method to myRio class to close the connection
        to the myRIO (2024/03/05)
 0.2.3: fixed the Default.lvbitx error: now the file is distributed 
        with the package. We use the relative folder of __file__ (2024/3/6)
 0.3.0: Added examples. Fixed a bug in the digital write function. (2024/3/7)
@@ -16,8 +16,9 @@
 1.1.0: MXP functions added to base, API and API client(2024/03/15)
 1.1.1: MXP function testing bugs fixed (2024/03/15)
 1.1.2: Bug fix: examples folder was not being copied to the site-packages (2024/03/15)
 1.2.1: Added play_waveform function to the myRIO class (2024/04/10)
 1.2.2: Minor fix in waveform example (2024/04/10)
 1.3.1: Added PWM capabilities (2024/04/12)
 1.3.2: Fixed minor bug (repeated API method) (2024/04/12)
+1.3.3: typing errors fixed (2024/04/15)
 """
```

### Comparing `myRIO_library-1.3.2/src/myRIO_API_client/examples/README_client.txt` & `myrio_library-1.3.3/src/myRIO_API_client/examples/README_client.txt`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/src/myRIO_API_client/examples/client_examples.py` & `myrio_library-1.3.3/src/myRIO_API_client/examples/client_examples.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/src/myRIO_API_client/myRIO_API_client.py` & `myrio_library-1.3.3/src/myRIO_API_client/myRIO_API_client.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/src/myRIO_API_client/version.py` & `myrio_library-1.3.3/src/myRIO_API_client/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # version.py
-__version__ = "1.3.2"
+__version__ = "1.3.3"
 
 """ version notes
 0.2.0: added __del__ method to myRio class to close the connection
        to the myRIO (2024/03/05)
 0.2.3: fixed the Default.lvbitx error: now the file is distributed 
        with the package. We use the relative folder of __file__ (2024/3/6)
 0.3.0: Added examples. Fixed a bug in the digital write function. (2024/3/7)
@@ -16,8 +16,9 @@
 1.1.0: MXP functions added to base, API and API client(2024/03/15)
 1.1.1: MXP function testing bugs fixed (2024/03/15)
 1.1.2: Bug fix: examples folder was not being copied to the site-packages (2024/03/15)
 1.2.1: Added play_waveform function to the myRIO class (2024/04/10)
 1.2.2: Minor fix in waveform example (2024/04/10)
 1.3.1: Added PWM capabilities (2024/04/12)
 1.3.2: Fixed minor bug (repeated API method) (2024/04/12)
+1.3.3: typing errors fixed (2024/04/15)
 """
```

### Comparing `myRIO_library-1.3.2/src/myRIO_base/data/Default.lvbitx` & `myrio_library-1.3.3/src/myRIO_base/data/Default.lvbitx`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/src/myRIO_base/data/High-throughput.lvbitx` & `myrio_library-1.3.3/src/myRIO_base/data/High-throughput.lvbitx`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/src/myRIO_base/examples/PWM_tests.py` & `myrio_library-1.3.3/src/myRIO_base/examples/PWM_tests.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/src/myRIO_base/examples/PacManDeath.csv` & `myrio_library-1.3.3/src/myRIO_base/examples/PacManDeath.csv`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/src/myRIO_base/examples/analog-inputs-and-outputs.py` & `myrio_library-1.3.3/src/myRIO_base/examples/analog-inputs-and-outputs.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/src/myRIO_base/examples/digital-inputs-and-outputs.py` & `myrio_library-1.3.3/src/myRIO_base/examples/digital-inputs-and-outputs.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/src/myRIO_base/examples/mxp-board-tests.py` & `myrio_library-1.3.3/src/myRIO_base/examples/mxp-board-tests.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/src/myRIO_base/examples/waveform-test.py` & `myrio_library-1.3.3/src/myRIO_base/examples/waveform-test.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.3.2/src/myRIO_base/myRIO_base.py` & `myrio_library-1.3.3/src/myRIO_base/myRIO_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 This library is an improvement over nifpga, a Python library that
 gives access to the FPGA registers of NI targets with FPGA.
 
 In this library, we have created some support functions and a class
 named MyRIO.
 """
 
-from nifpga import Session
-from typing import Tuple
+from nifpga import Session # type: ignore
+from typing import Tuple, List
 import ctypes
 import pkg_resources
 
 
 # RGB constants
 
 RED = 2
@@ -21,15 +21,15 @@
 WHITE = 7
 RGB_OFF = 0
 
 
 # Support functions. They are not part of the class MyRIO, but they are used by it.
 # Feel free to use them in your own programs.
 
-def u8_to_bits (u8_number: int) -> [bool]:
+def u8_to_bits (u8_number: int) -> List[bool]:
     """ This function converts u8 values to an array of Booleans """
     mask = 1
     one_by_one = []
     for i in range(8):
         one_by_one.append(bool((u8_number & mask) != 0))
         mask = mask * 2
     return(one_by_one)
@@ -105,15 +105,15 @@
 
 def volts_to_luminosity (volts: float) -> float:
     """ This function converts values in Volts 
     to luminosity in percentage (0-100%)
     """
     return 100-(volts*30.3)
 
-def extract_waveform_from_csv_file(file_name: str) -> [int]:
+def extract_waveform_from_csv_file(file_name: str) -> List[int]:
     """ This function extracts a stereo waveform from a .csv file
     and returns it as a list of I16 integers.
     The .csv format is very basic for an audio file, but
     the myRIO has memory limitations, so the audio files
     must be mono and quite shorts.
     We have tried the wave library from Python, but it does not work
     properly with the myRIO, so we have used the csv format that 
@@ -142,16 +142,17 @@
     def __init__(self, session_bitfile="", session_resource = "RIO0"):
         """ when an instance is created, an nifpga session is created. """
         if session_bitfile == "":
             session_bitfile = pkg_resources.resource_filename('myRIO_base', 'data/Default.lvbitx')
 
         self.__session = Session(session_bitfile, session_resource)
         sys_handler = self.__session.registers['SYS.RDY']
+        from time import sleep
         while not sys_handler.read():       #TODO: What if the system is never ready?
-            time.sleep(0.1)
+            sleep(0.1)
 
     def check_if_ready(self) -> bool:
         """ checks if system is ready """
         sys_handler = self.__session.registers['SYS.RDY']
         return sys_handler.read()
 
     def __del__(self):
@@ -168,15 +169,15 @@
         dir_string_high = 'DIO.' + port + '_' + '15:8' + '.DIR'
         mask_handler_low = self.__session.registers[dir_string_low]
         mask_handler_high = self.__session.registers[dir_string_high]
         mask_handler_low.write(mask_low)    # 7 is 00000111 where 1 is OUT
         mask_handler_high.write(mask_high)    # 0 is 00000000 where 0 is IN
 
     def update_DIO_mask(self, channel: int, is_output: bool, port: str ='A'):
-        """ Updates the current DIO mask to change the behaviour of one channe """
+        """ Updates the current DIO mask to change the behaviour of one channel """
 
         dir_string_low = 'DIO.' + port + '_' + '7:0' + '.DIR'
         dir_string_high = 'DIO.' + port + '_' + '15:8' + '.DIR'
         mask_handler_low = self.__session.registers[dir_string_low]
         mask_handler_high = self.__session.registers[dir_string_high]
         current_dio_mask_low = mask_handler_low.read()
         current_dio_mask_high = mask_handler_high.read()
@@ -249,15 +250,15 @@
             array_index = channel-8
 
         channel_handler = self.__session.registers[channel_string]
         raw_value = channel_handler.read()
         bool_array = u8_to_bits(raw_value)
         return bool_array[array_index]
 
-    def read_digital_port(self, port: str ='A') -> [bool]:
+    def read_digital_port(self, port: str ='A') -> List[bool]:
         """ returns the Boolean values of the whole port (default port: A) """
 
         channel_string_low = 'DIO.' + port + '_7:0.IN'
         channel_string_high = 'DIO.' + port + '_15:8.IN'
         channel_handler_low = self.__session.registers[channel_string_low]
         channel_handler_high = self.__session.registers[channel_string_high]
         raw_value_low = channel_handler_low.read()
@@ -319,15 +320,15 @@
         """ changes the state of the myRIO onboard LEDs using an integer value """
 
         value = max(0, min(raw_value, 15))      #TODO: raising a warning when out of range?
         channel_string = 'DO.LED3:0'
         channel_handler = self.__session.registers[channel_string]
         channel_handler.write(value)
 
-    def write_leds_booleans(self, boolean_values: [bool]):
+    def write_leds_booleans(self, boolean_values: List[bool]):
         """ changes the state of the myRIO onboard LEDs using Booleans """
 
         raw_value = 0
         j = 1
         for i in range(4):
             raw_value = raw_value + boolean_values[i]*j
             j = j*2
@@ -446,15 +447,15 @@
         
         channel_handler = self.__session.registers[channel_string]
         raw_value = volts_to_raw_audio(value)
         channel_handler.write(raw_value)
         go_handler = self.__session.registers['AO.SYS.GO']
         go_handler.write(True)
 
-    def play_waveform(self, waveform: [int]):
+    def play_waveform(self, waveform: List[int]):
         """ plays a waveform on the myRIO Audio Output channels """
     
         channel_string_left = 'AO.AudioOut_L.VAL'
         channel_string_right = 'AO.AudioOut_R.VAL'
         channel_handler_left = self.__session.registers[channel_string_left]
         channel_handler_right = self.__session.registers[channel_string_right]
```

### Comparing `myRIO_library-1.3.2/src/myRIO_base/version.py` & `myrio_library-1.3.3/src/myRIO_base/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # version.py
-__version__ = "1.3.2"
+__version__ = "1.3.3"
 
 """ version notes
 0.2.0: added __del__ method to myRio class to close the connection
        to the myRIO (2024/03/05)
 0.2.3: fixed the Default.lvbitx error: now the file is distributed 
        with the package. We use the relative folder of __file__ (2024/3/6)
 0.3.0: Added examples. Fixed a bug in the digital write function. (2024/3/7)
@@ -16,8 +16,9 @@
 1.1.0: MXP functions added to base, API and API client(2024/03/15)
 1.1.1: MXP function testing bugs fixed (2024/03/15)
 1.1.2: Bug fix: examples folder was not being copied to the site-packages (2024/03/15)
 1.2.1: Added play_waveform function to the myRIO class (2024/04/10)
 1.2.2: Minor fix in waveform example (2024/04/10)
 1.3.1: Added PWM capabilities (2024/04/12)
 1.3.2: Fixed minor bug (repeated API method) (2024/04/12)
+1.3.3: typing errors fixed (2024/04/15)
 """
```

### Comparing `myRIO_library-1.3.2/src/myRIO_library.egg-info/PKG-INFO` & `myrio_library-1.3.3/src/myRIO_library.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myRIO_library
-Version: 1.3.2
+Version: 1.3.3
 Summary: A library to control the myRIO board from National Instruments
 Home-page: https://github.com/AitzolEzeizaUPVEHU/myRIO_library
 Download-URL: https://github.com/AitzolEzeizaUPVEHU/myRIO_library/archive/refs/heads/main.zip
 Author: Aitzol Ezeiza Ramos
 Author-email: aitzol.ezeiza@ehu.eus
 License: MIT
 Keywords: myRIO,NI,National Instruments,LabVIEW,Python,FPGA,Real-Time,Embedded Systems
```

### Comparing `myRIO_library-1.3.2/src/myRIO_library.egg-info/SOURCES.txt` & `myrio_library-1.3.3/src/myRIO_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

