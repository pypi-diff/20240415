# Comparing `tmp/moku-3.1.1.tar.gz` & `tmp/moku-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moku-3.1.1.tar", last modified: Fri Nov  3 05:10:02 2023, max compression
+gzip compressed data, was "moku-3.2.0.tar", last modified: Mon Apr 15 02:40:24 2024, max compression
```

## Comparing `moku-3.1.1.tar` & `moku-3.2.0.tar`

### file list

```diff
@@ -1,39 +1,45 @@
-drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-11-03 05:10:02.839768 moku-3.1.1/
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     1146 2023-11-03 05:10:02.839768 moku-3.1.1/PKG-INFO
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     2674 2022-12-12 03:43:28.000000 moku-3.1.1/README.md
-drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-11-03 05:10:02.839768 moku-3.1.1/moku/
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    11191 2023-11-03 01:44:26.000000 moku-3.1.1/moku/__init__.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     3831 2023-11-03 01:44:26.000000 moku-3.1.1/moku/cli.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     1672 2023-01-27 07:08:13.000000 moku-3.1.1/moku/exceptions.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     4353 2022-12-12 03:43:28.000000 moku-3.1.1/moku/finder.py
-drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-11-03 05:10:02.839768 moku-3.1.1/moku/instruments/
--rw-rw-r--   0 sashi     (1001) sashi     (1001)      736 2023-11-03 01:44:26.000000 moku-3.1.1/moku/instruments/__init__.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    12971 2023-11-03 04:59:52.000000 moku-3.1.1/moku/instruments/_awg.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     5819 2023-11-03 01:44:26.000000 moku-3.1.1/moku/instruments/_cloudcompile.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    15841 2023-11-03 04:59:52.000000 moku-3.1.1/moku/instruments/_datalogger.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    30163 2023-11-03 04:59:52.000000 moku-3.1.1/moku/instruments/_digitalfilterbox.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    35526 2023-11-03 04:59:52.000000 moku-3.1.1/moku/instruments/_firfilter.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    16388 2023-11-03 04:59:52.000000 moku-3.1.1/moku/instruments/_fra.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    36409 2023-11-03 04:59:52.000000 moku-3.1.1/moku/instruments/_laserlockbox.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    29003 2023-11-03 04:59:52.000000 moku-3.1.1/moku/instruments/_lockinamp.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    25385 2023-11-03 04:59:52.000000 moku-3.1.1/moku/instruments/_logicanalyzer.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     6189 2023-11-03 01:44:26.000000 moku-3.1.1/moku/instruments/_mim.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    26241 2023-11-03 04:59:52.000000 moku-3.1.1/moku/instruments/_oscilloscope.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    17948 2023-11-03 01:44:26.000000 moku-3.1.1/moku/instruments/_phasemeter.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    31253 2023-11-03 04:59:52.000000 moku-3.1.1/moku/instruments/_pidcontroller.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    13638 2023-11-03 01:44:26.000000 moku-3.1.1/moku/instruments/_spectrumanalyzer.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     5181 2023-11-03 05:06:15.000000 moku-3.1.1/moku/instruments/_stream.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    16925 2023-11-03 04:59:52.000000 moku-3.1.1/moku/instruments/_waveformgenerator.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     6181 2023-11-03 01:44:26.000000 moku-3.1.1/moku/session.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     1452 2023-11-03 01:44:26.000000 moku-3.1.1/moku/utilities.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)      277 2023-11-03 01:44:26.000000 moku-3.1.1/moku/version.py
-drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-11-03 05:10:02.839768 moku-3.1.1/moku.egg-info/
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     1146 2023-11-03 05:10:02.000000 moku-3.1.1/moku.egg-info/PKG-INFO
--rw-rw-r--   0 sashi     (1001) sashi     (1001)      883 2023-11-03 05:10:02.000000 moku-3.1.1/moku.egg-info/SOURCES.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)        1 2023-11-03 05:10:02.000000 moku-3.1.1/moku.egg-info/dependency_links.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)       40 2023-11-03 05:10:02.000000 moku-3.1.1/moku.egg-info/entry_points.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)        1 2023-01-27 05:59:57.000000 moku-3.1.1/moku.egg-info/not-zip-safe
--rw-rw-r--   0 sashi     (1001) sashi     (1001)       26 2023-11-03 05:10:02.000000 moku-3.1.1/moku.egg-info/requires.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)        5 2023-11-03 05:10:02.000000 moku-3.1.1/moku.egg-info/top_level.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)       38 2023-11-03 05:10:02.843768 moku-3.1.1/setup.cfg
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     1598 2023-11-03 01:44:26.000000 moku-3.1.1/setup.py
+drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2024-04-15 02:40:24.450239 moku-3.2.0/
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1094 2024-04-15 02:38:47.000000 moku-3.2.0/LICENSE.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1146 2024-04-15 02:40:24.450239 moku-3.2.0/PKG-INFO
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     2674 2022-12-12 03:43:28.000000 moku-3.2.0/README.md
+drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2024-04-15 02:40:24.446239 moku-3.2.0/moku/
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    11842 2024-04-15 02:38:47.000000 moku-3.2.0/moku/__init__.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     3831 2023-11-03 01:44:26.000000 moku-3.2.0/moku/cli.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1672 2023-01-27 07:08:13.000000 moku-3.2.0/moku/exceptions.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     4353 2022-12-12 03:43:28.000000 moku-3.2.0/moku/finder.py
+drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2024-04-15 02:40:24.446239 moku-3.2.0/moku/instruments/
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)      784 2024-04-15 02:38:47.000000 moku-3.2.0/moku/instruments/__init__.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    12971 2023-11-03 04:59:52.000000 moku-3.2.0/moku/instruments/_awg.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     5819 2023-11-03 01:44:26.000000 moku-3.2.0/moku/instruments/_cloudcompile.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    16857 2024-04-15 02:38:47.000000 moku-3.2.0/moku/instruments/_datalogger.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    31023 2024-04-15 02:38:47.000000 moku-3.2.0/moku/instruments/_digitalfilterbox.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    36385 2024-04-15 02:38:47.000000 moku-3.2.0/moku/instruments/_firfilter.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    16388 2023-11-03 04:59:52.000000 moku-3.2.0/moku/instruments/_fra.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    37221 2024-04-15 02:38:47.000000 moku-3.2.0/moku/instruments/_laserlockbox.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    29863 2024-04-15 02:38:47.000000 moku-3.2.0/moku/instruments/_lockinamp.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    27492 2024-04-15 02:38:47.000000 moku-3.2.0/moku/instruments/_logicanalyzer.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     6189 2023-11-03 01:44:26.000000 moku-3.2.0/moku/instruments/_mim.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    26241 2024-03-18 22:58:10.000000 moku-3.2.0/moku/instruments/_oscilloscope.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    19045 2024-04-15 02:38:47.000000 moku-3.2.0/moku/instruments/_phasemeter.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    32113 2024-04-15 02:38:47.000000 moku-3.2.0/moku/instruments/_pidcontroller.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    15335 2024-04-15 02:38:47.000000 moku-3.2.0/moku/instruments/_spectrumanalyzer.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     5570 2024-04-15 02:38:47.000000 moku-3.2.0/moku/instruments/_stream.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    15645 2024-04-15 02:38:47.000000 moku-3.2.0/moku/instruments/_tfa.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    17059 2024-04-15 02:38:47.000000 moku-3.2.0/moku/instruments/_waveformgenerator.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     6598 2024-04-15 02:38:47.000000 moku-3.2.0/moku/session.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1452 2024-04-02 23:59:59.000000 moku-3.2.0/moku/utilities.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)      277 2024-04-05 04:58:37.000000 moku-3.2.0/moku/version.py
+drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2024-04-15 02:40:24.446239 moku-3.2.0/moku.egg-info/
+-rw-r--r--   0 sashi     (1001) sashi     (1001)     1146 2024-04-15 02:40:24.000000 moku-3.2.0/moku.egg-info/PKG-INFO
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)      969 2024-04-15 02:40:24.000000 moku-3.2.0/moku.egg-info/SOURCES.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)        1 2024-04-15 02:40:24.000000 moku-3.2.0/moku.egg-info/dependency_links.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)       40 2024-04-15 02:40:24.000000 moku-3.2.0/moku.egg-info/entry_points.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)        1 2024-04-09 00:25:53.000000 moku-3.2.0/moku.egg-info/not-zip-safe
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)       26 2024-04-15 02:40:24.000000 moku-3.2.0/moku.egg-info/requires.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)        5 2024-04-15 02:40:24.000000 moku-3.2.0/moku.egg-info/top_level.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1559 2024-04-08 03:56:33.000000 moku-3.2.0/pyproject.toml
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)       38 2024-04-15 02:40:24.450239 moku-3.2.0/setup.cfg
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1598 2024-04-15 02:38:47.000000 moku-3.2.0/setup.py
+drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2024-04-15 02:40:24.446239 moku-3.2.0/tests/
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1376 2023-09-15 01:09:31.000000 moku-3.2.0/tests/test(2).py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)      812 2023-09-06 05:35:08.000000 moku-3.2.0/tests/test_dl.py
```

### Comparing `moku-3.1.1/PKG-INFO` & `moku-3.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moku
-Version: 3.1.1
+Version: 3.2.0
 Summary: Python scripting interface to the Liquid Instruments Moku hardware
 Home-page: https://liquidinstruments.com
 Author: Liquid Instruments
 Author-email: info@liquidinstruments.com
 License: MIT
 Description: 
                 # Moku
```

### Comparing `moku-3.1.1/README.md` & `moku-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `moku-3.1.1/moku/__init__.py` & `moku-3.2.0/moku/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from hashlib import sha256
 from os import environ
 from pathlib import Path
 from shutil import which
 
 from pkg_resources import get_distribution, resource_filename
 
-from moku.exceptions import IncompatibleMokuException, MokuException
+from moku.exceptions import (
+    IncompatibleMokuException,
+    MokuException,
+    NoInstrumentBitstream
+)
 from moku.session import RequestSession
 from moku.utilities import validate_range
 from moku.version import MIN_COMPAT_FW, COMPAT_FW
 
 __version__ = get_distribution("moku").version
 _data_path = environ.get('MOKU_DATA_PATH',
                          resource_filename("moku", 'data'))
@@ -19,14 +23,19 @@
 
 MOKU_CLI_PATH = environ.get('MOKU_CLI_PATH', which("mokucli"))
 if MOKU_CLI_PATH:
     MOKU_CLI_PATH = str(Path(MOKU_CLI_PATH).expanduser())
 
 
 class Moku:
+    """
+    Moku base class. This class does all the heavy lifting required to 
+    deploy and control instruments.
+    """
+
     def __init__(self, ip, force_connect, ignore_busy,
                  persist_state, connect_timeout,
                  read_timeout, **kwargs):
         self.session = RequestSession(ip, connect_timeout,
                                       read_timeout, **kwargs)
         self.claim_ownership(force_connect, ignore_busy,
                              persist_state)
@@ -39,15 +48,15 @@
                 f"package supports firmware version"
                 f"{MIN_COMPAT_FW} or above.")
 
         if int(props['firmware']) < COMPAT_FW:
             print(
                 "You are using an old version of Moku firmware. "
                 "Some features may not work properly. "
-                "Please update your firmware to the latest version using the Moku Desktop app.") # noqa
+                "Please update your firmware to the latest version using the Moku Desktop app.")  # noqa
 
         self.firmware_version = props['firmware']
         self.hardware = props['hardware'].replace(":", "").lower()
         self.bitstreams = props['bitstreams']
 
     def _read_and_upload_stream(self, bs_name, chksum, bs_path=None):
         if bs_path:
@@ -73,48 +82,48 @@
 
     def upload_bitstream(self, name, bs_path=None):
         matching = [b for b in self.bitstreams if b["name"] == name]
         chksum = matching[0].get("checksum") if matching else None
         self._read_and_upload_stream(name, chksum, bs_path)
 
     def set_connect_timeout(self, value):
+        "Sets requests session connect timeout"
         if not isinstance(value, tuple([int, float])):
-            raise Exception("set_connect_timeout value should be "
-                            "either integer or float")
+            raise ValueError("set_connect_timeout value should be "
+                             "either integer or float")
         self.session.connect_timeout = value
 
     def set_read_timeout(self, value):
+        "Sets requests session read timeout"
         if not isinstance(value, tuple([int, float])):
-            raise Exception("read_timeout value should be either "
-                            "integer or float")
+            raise ValueError("read_timeout value should be either "
+                             "integer or float")
         self.session.read_timeout = value
 
     def platform(self, platform_id):
+        "Configures platform for the given ID"
         platform_map = {"mokupro": [1, 4],
                         "mokugo": [1, 2],
                         "mokulab": [1, 2]}
         if platform_id not in platform_map[self.hardware]:
-            raise MokuException(f"The platform_id {platform_id} is invalid. For '{self.hardware}' available options are {platform_map[self.hardware]}") # noqa
+            raise MokuException(f"The platform_id {platform_id} is invalid. For '{self.hardware}' available options are {platform_map[self.hardware]}")  # noqa
 
         operation = f"platform/{platform_id}"
         self.upload_bitstream(f"{platform_id:02}-000")
         for i in range(0, platform_id):
             self.upload_bitstream(f"{platform_id:02}-000-{i:02}")
         return self.session.get("moku", operation)
 
     @staticmethod
     def _get_data_file(firmware_version):
         file_name = f'mokudata-{firmware_version}.tar.gz'
         path = MOKU_DATA_PATH.joinpath(file_name)
         if not path.exists():
-            raise Exception(
-                'Instrument files not available, please run '
-                '`moku download --fw_ver={}` to '
-                'download latest instrument data'.format(
-                    firmware_version))
+            raise NoInstrumentBitstream(
+                f'Instrument files not available, please run `moku download --fw_ver={firmware_version}` to download latest instrument data')  # noqa
         return path
 
     def claim_ownership(
             self,
             force_connect=True,
             ignore_busy=False,
             persist_state=False):
@@ -292,16 +301,14 @@
         """
         List files at bitstreams, ssd, logs, persist.
 
         :type target: `string`, (bitstreams, ssd, logs, persist, media)
         :param target: Target directory to list files for
 
         """
-        target = validate_range(target, list(
-            ['bitstreams', 'ssd', 'logs', 'persist', 'media']))
         operation = "list"
         return self.session.get(target, operation)
 
     def download(self, target, file_name, local_path):
         """
         Download files from bitstreams, ssd, logs, persist.
 
@@ -316,21 +323,37 @@
 
         """
         target = validate_range(target, list(
             ['bitstreams', 'ssd', 'logs', 'persist', 'media']))
         operation = f"download/{file_name}"
         return self.session.get_file(target, operation, local_path)
 
-    def _modify_config(self, data=None):
+    def modify_hardware(self, data=None):
+        """
+        CAUTION: Never use to update the state of the Moku
+        Raw access to Moku hardware state
+        """
         if data is None:
             data = {}
-        return self.session.post_to_v2("config", data)
+        return self.session.post("moku", "modify_hardware", data)
 
-    def _modify_hardware(self, data=None):
+    def modify_calibration(self, data=None):
+        """
+        Query or update the calibration coefficients
+        """
         if data is None:
             data = {}
-        return self.session.post_to_v2("hwstate", data)
+        return self.session.post("moku", "modify_calibration", data)
 
-    def _calibrate(self, data=None):
+    def set_configuration(self, data=None):
+        """
+        Update the Moku device/network configuration.
+        """
         if data is None:
             data = {}
-        return self.session.post_to_v2("calibration", data)
+        return self.session.post("moku", "modify_calibration", data)
+
+    def get_configuration(self):
+        """
+        Retreive the Moku device/network configuration.
+        """
+        return self.session.get("moku", "get_configuration")
```

### Comparing `moku-3.1.1/moku/cli.py` & `moku-3.2.0/moku/cli.py`

 * *Files identical despite different names*

### Comparing `moku-3.1.1/moku/exceptions.py` & `moku-3.2.0/moku/exceptions.py`

 * *Files identical despite different names*

### Comparing `moku-3.1.1/moku/finder.py` & `moku-3.2.0/moku/finder.py`

 * *Files identical despite different names*

### Comparing `moku-3.1.1/moku/instruments/__init__.py` & `moku-3.2.0/moku/instruments/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,7 +9,8 @@
 from ._logicanalyzer import LogicAnalyzer  # noqa
 from ._mim import MultiInstrument  # noqa
 from ._oscilloscope import Oscilloscope  # noqa
 from ._phasemeter import Phasemeter  # noqa
 from ._pidcontroller import PIDController  # noqa
 from ._spectrumanalyzer import SpectrumAnalyzer  # noqa
 from ._waveformgenerator import WaveformGenerator  # noqa
+from ._tfa import TimeFrequencyAnalyzer  # noqa
```

### Comparing `moku-3.1.1/moku/instruments/_awg.py` & `moku-3.2.0/moku/instruments/_awg.py`

 * *Files identical despite different names*

### Comparing `moku-3.1.1/moku/instruments/_cloudcompile.py` & `moku-3.2.0/moku/instruments/_cloudcompile.py`

 * *Files identical despite different names*

### Comparing `moku-3.1.1/moku/instruments/_datalogger.py` & `moku-3.2.0/moku/instruments/_datalogger.py`

 * *Files 8% similar despite different names*

```diff
@@ -222,27 +222,35 @@
 
     def start_logging(
             self,
             duration=60,
             delay=0,
             file_name_prefix="",
             comments="",
+            trigger_source=None,
+            trigger_level=None,
             strict=True):
         """
         start_logging.
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
 
-        :type duration: `integer` Sec (defaults to 60)
+        :type duration: `double` Sec (defaults to 60)
         :param duration: Duration to log for
 
         :type delay: `integer` Sec (defaults to 0)
         :param delay: Delay the start by
 
+        :type trigger_source: `string` ['ChannelA', 'ChannelB', 'ChannelC', 'ChannelD', 'Input1', 'Input2', 'Input3', 'Input4', 'Output1', 'Output2', 'Output3', 'Output4', 'External'] # noqa
+        :param trigger_source: Trigger source
+
+        :type trigger_level: `number` [-5V, 5V]  (defaults to 0)
+        :param trigger_level: Trigger level
+
         :type file_name_prefix: `string`
         :param file_name_prefix: Optional file name prefix
 
         :type comments: `string`
         :param comments: Optional comments to be included
 
 
@@ -252,14 +260,16 @@
 
         """
         operation = "start_logging"
         params = dict(
             strict=strict,
             duration=duration,
             delay=delay,
+            trigger_source=trigger_source,
+            trigger_level=trigger_level,
             file_name_prefix=file_name_prefix,
             comments=comments,
         )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
@@ -459,30 +469,40 @@
         """
         logging_progress.
         """
         operation = "logging_progress"
         return self.session.get(
             f"slot{self.slot}/{self.operation_group}", operation)
 
-    def start_streaming(self, duration=None, sample_rate=None):
+    def start_streaming(self, duration=None, sample_rate=None,
+                        trigger_source=None,
+                        trigger_level=None):
         """
         start_streaming.
 
-        :type duration: `integer`
+        :type duration: `double`
         :param duration: Duration in second(s) to stream for
 
         :type sample_rate: `number` [10, 1e6]
         :param sample_rate: Target samples per second
 
+        :type trigger_source: `string` ['ChannelA', 'ChannelB', 'ChannelC', 'ChannelD', 'Input1', 'Input2', 'Input3', 'Input4', 'Output1', 'Output2', 'Output3', 'Output4', 'External'] # noqa
+        :param trigger_source: Trigger source
+
+        :type trigger_level: `number` [-5V, 5V]  (defaults to 0)
+        :param trigger_level: Trigger level
+
         """
         super().start_streaming()
         operation = "start_streaming"
         params = dict(
             duration=duration,
-            sample_rate=sample_rate
+            sample_rate=sample_rate,
+            trigger_source=trigger_source,
+            trigger_level=trigger_level
         )
         response = self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
         self.stream_id = response["stream_id"]
         self.ip_address = self.session.ip_address
```

### Comparing `moku-3.1.1/moku/instruments/_digitalfilterbox.py` & `moku-3.2.0/moku/instruments/_digitalfilterbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,15 +384,15 @@
 
         :type noise_reject: `boolean`
         :param noise_reject: Configure the Oscilloscope with a small amount of hysteresis to prevent repeated triggering due to noise # noqa
 
         :type hf_reject: `boolean`
         :param hf_reject: Configure the trigger signal to pass through a low pass filter to smooths out the noise # noqa
 
-        :type source: `string` ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD']
+        :type source: `string` ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External']
         :param source: Trigger Source
 
         """
         operation = "set_trigger"
         params = dict(
             strict=strict,
             type=validate_range(type, ['Edge', 'Pulse']),
@@ -406,15 +406,15 @@
             nth_event=nth_event,
             holdoff=holdoff,
             hysteresis=hysteresis,
             auto_sensitivity=auto_sensitivity,
             noise_reject=noise_reject,
             hf_reject=hf_reject,
             source=validate_range(
-                source, ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD']),
+                source, ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External']),
         )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
 
     def set_filter(
@@ -829,14 +829,16 @@
 
     def start_logging(
             self,
             duration=60,
             delay=0,
             file_name_prefix="",
             comments="",
+            trigger_source=None,
+            trigger_level=None,
             mode="Normal",
             rate=1000,
             strict=True):
         """
         start_logging.
 
         :type strict: `boolean`
@@ -844,14 +846,20 @@
 
         :type duration: `integer` Sec (defaults to 60)
         :param duration: Duration to log for
 
         :type delay: `integer` Sec (defaults to 0)
         :param delay: Delay the start by
 
+        :type trigger_source: `string`  ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External'] # noqa
+        :param trigger_source: Trigger source
+
+        :type trigger_level: `number` [-5V, 5V]  (defaults to 0)
+        :param trigger_level: Trigger level
+
         :type file_name_prefix: `string`
         :param file_name_prefix: Optional file name prefix
 
         :type comments: `string`
         :param comments: Optional comments to be included
 
         :type mode: `string` ['Normal', 'Precision', 'DeepMemory', 'PeakDetect'] # noqa
@@ -862,14 +870,16 @@
 
         """
         operation = "start_logging"
         params = dict(
             strict=strict,
             duration=duration,
             delay=delay,
+            trigger_source=trigger_source,
+            trigger_level=trigger_level,
             file_name_prefix=file_name_prefix,
             comments=comments,
             mode=validate_range(
                 mode, ['Normal', 'Precision', 'DeepMemory', 'PeakDetect']),
             rate=rate,
         )
         return self.session.post(
@@ -881,35 +891,46 @@
         """
         stop_logging.
         """
         operation = "stop_logging"
         return self.session.get(
             f"slot{self.slot}/{self.operation_group}", operation)
 
-    def start_streaming(self, duration=None, mode="Normal", rate=1000):
+    def start_streaming(self, duration=None, mode="Normal", rate=1000,
+                        trigger_source=None,
+                        trigger_level=None):
         """
         start_streaming.
 
         :type duration: `integer`
         :param duration: Duration in second(s) to stream for
 
         :type mode: `string` ['Normal', 'Precision', 'DeepMemory', 'PeakDetect'] # noqa
         :param mode: Acquisition Mode
 
         :type rate: `number`
         :param rate: Acquisition rate
 
+        :type trigger_source: `string`  ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External'] # noqa
+        :param trigger_source: Trigger source
+
+        :type trigger_level: `number` [-5V, 5V]  (defaults to 0)
+        :param trigger_level: Trigger level
+
+
         """
         super().start_streaming()
         operation = "start_streaming"
         params = dict(
             duration=duration,
             mode=validate_range(
                 mode, ['Normal', 'Precision', 'DeepMemory', 'PeakDetect']),
             rate=rate,
+            trigger_source=trigger_source,
+            trigger_level=trigger_level
         )
 
         response = self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
         self.stream_id = response["stream_id"]
```

### Comparing `moku-3.1.1/moku/instruments/_firfilter.py` & `moku-3.2.0/moku/instruments/_firfilter.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,15 +383,15 @@
 
         :type noise_reject: `boolean`
         :param noise_reject: Configure the Oscilloscope with a small amount of hysteresis to prevent repeated triggering due to noise # noqa
 
         :type hf_reject: `boolean`
         :param hf_reject: Configure the trigger signal to pass through a low pass filter to smooths out the noise # noqa
 
-        :type source: `string` ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD']
+        :type source: `string` ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External']
         :param source: Trigger Source
 
         """
         operation = "set_trigger"
         params = dict(
             strict=strict,
             type=validate_range(type, ['Edge', 'Pulse']),
@@ -405,15 +405,15 @@
             nth_event=nth_event,
             holdoff=holdoff,
             hysteresis=hysteresis,
             auto_sensitivity=auto_sensitivity,
             noise_reject=noise_reject,
             hf_reject=hf_reject,
             source=validate_range(
-                source, ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD']),
+                source, ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD','External']),
         )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
 
     def set_by_frequency(
@@ -928,14 +928,16 @@
 
     def start_logging(
             self,
             duration=60,
             delay=0,
             file_name_prefix="",
             comments="",
+            trigger_source=None,
+            trigger_level=None,
             mode="Normal",
             rate=1000,
             strict=True):
         """
         start_logging.
 
         :type strict: `boolean`
@@ -943,14 +945,20 @@
 
         :type duration: `integer` Sec (defaults to 60)
         :param duration: Duration to log for
 
         :type delay: `integer` Sec (defaults to 0)
         :param delay: Delay the start by
 
+        :type trigger_source: `string`  ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External'] # noqa
+        :param trigger_source: Trigger source
+
+        :type trigger_level: `number` [-5V, 5V]  (defaults to 0)
+        :param trigger_level: Trigger level
+
         :type file_name_prefix: `string`
         :param file_name_prefix: Optional file name prefix
 
         :type comments: `string`
         :param comments: Optional comments to be included
 
         :type mode: `string` ['Normal', 'Precision', 'DeepMemory', 'PeakDetect'] # noqa
@@ -961,14 +969,16 @@
 
         """
         operation = "start_logging"
         params = dict(
             strict=strict,
             duration=duration,
             delay=delay,
+            trigger_source=trigger_source,
+            trigger_level=trigger_level,
             file_name_prefix=file_name_prefix,
             comments=comments,
             mode=validate_range(
                 mode, ['Normal', 'Precision', 'DeepMemory', 'PeakDetect']),
             rate=rate,
         )
         return self.session.post(
@@ -980,35 +990,46 @@
         """
         stop_logging.
         """
         operation = "stop_logging"
         return self.session.get(
             f"slot{self.slot}/{self.operation_group}", operation)
 
-    def start_streaming(self, duration=None, mode="Normal", rate=1000):
+    def start_streaming(self, duration=None, mode="Normal", rate=1000,
+                        trigger_source=None,
+                        trigger_level=None):
         """
         start_streaming.
 
         :type duration: `integer`
         :param duration: Duration in second(s) to stream for
 
         :type mode: `string` ['Normal', 'Precision', 'DeepMemory', 'PeakDetect'] # noqa
         :param mode: Acquisition Mode
 
         :type rate: `number`
         :param rate: Acquisition rate
 
+        :type trigger_source: `string`  ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External'] # noqa
+        :param trigger_source: Trigger source
+
+        :type trigger_level: `number` [-5V, 5V]  (defaults to 0)
+        :param trigger_level: Trigger level
+
+
         """
         super().start_streaming()
         operation = "start_streaming"
         params = dict(
             duration=duration,
             mode=validate_range(
                 mode, ['Normal', 'Precision', 'DeepMemory', 'PeakDetect']),
             rate=rate,
+            trigger_source=trigger_source,
+            trigger_level=trigger_level
         )
 
         response = self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
         self.stream_id = response["stream_id"]
```

### Comparing `moku-3.1.1/moku/instruments/_fra.py` & `moku-3.2.0/moku/instruments/_fra.py`

 * *Files identical despite different names*

### Comparing `moku-3.1.1/moku/instruments/_laserlockbox.py` & `moku-3.2.0/moku/instruments/_laserlockbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,21 +85,22 @@
 
         :type gain: `string` ['48dB', '24dB', '0dB', '-20dB', '-40dB']
         :param gain: Input gain
 
         """
         operation = "set_frontend"
         params = dict(
-            strict=strict, channel=channel, coupling=validate_range(
-                coupling, [
-                    'AC', 'DC']), impedance=validate_range(
-                impedance, [
-                    '1MOhm', '50Ohm']), gain=validate_range(
-                        gain, [
-                            '48dB', '24dB', '0dB', '-20dB', '-40dB']), )
+            strict=strict,
+            channel=channel,
+            coupling=validate_range(
+                coupling, ['AC', 'DC']),
+            impedance=validate_range(impedance, ['1MOhm', '50Ohm']),
+            gain=validate_range(
+                gain,
+                ['48dB', '24dB', '0dB', '-14dB', '-20dB', '-40dB']))
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
 
     def set_monitor(self, monitor_channel, source, strict=True):
         """
@@ -461,15 +462,15 @@
         :param phase: Demodulation signal phase
 
         """
         operation = "set_demodulation"
         params = dict(
             strict=strict,
             mode=validate_range(
-                mode, ['Modulation', 'Internal', 'External', 'ExternalPLL', 'None']), # noqa
+                mode, ['Modulation', 'Internal', 'External', 'ExternalPLL', 'None']),  # noqa
             frequency=frequency,
             phase=phase,
         )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
@@ -1000,14 +1001,16 @@
 
     def start_logging(
             self,
             duration=60,
             delay=0,
             file_name_prefix="",
             comments="",
+            trigger_source=None,
+            trigger_level=None,
             mode="Normal",
             rate=1000,
             strict=True):
         """
         start_logging.
 
         :type strict: `boolean`
@@ -1015,14 +1018,20 @@
 
         :type duration: `integer` Sec (defaults to 60)
         :param duration: Duration to log for
 
         :type delay: `integer` Sec (defaults to 0)
         :param delay: Delay the start by
 
+        :type trigger_source: `string`  ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External'] # noqa
+        :param trigger_source: Trigger source
+
+        :type trigger_level: `number` [-5V, 5V]  (defaults to 0)
+        :param trigger_level: Trigger level
+
         :type file_name_prefix: `string`
         :param file_name_prefix: Optional file name prefix
 
         :type comments: `string`
         :param comments: Optional comments to be included
 
         :type mode: `string` ['Normal', 'Precision', 'DeepMemory', 'PeakDetect'] # noqa
@@ -1033,14 +1042,16 @@
 
         """
         operation = "start_logging"
         params = dict(
             strict=strict,
             duration=duration,
             delay=delay,
+            trigger_source=trigger_source,
+            trigger_level=trigger_level,
             file_name_prefix=file_name_prefix,
             comments=comments,
             mode=validate_range(
                 mode, ['Normal', 'Precision', 'DeepMemory', 'PeakDetect']),
             rate=rate,
         )
         return self.session.post(
@@ -1052,35 +1063,46 @@
         """
         stop_logging.
         """
         operation = "stop_logging"
         return self.session.get(
             f"slot{self.slot}/{self.operation_group}", operation)
 
-    def start_streaming(self, duration=None, mode="Normal", rate=1000):
+    def start_streaming(self, duration=None, mode="Normal", rate=1000,
+                        trigger_source=None,
+                        trigger_level=None):
         """
         start_streaming.
 
         :type duration: `integer`
         :param duration: Duration in second(s) to stream for
 
         :type mode: `string` ['Normal', 'Precision', 'DeepMemory', 'PeakDetect'] # noqa
         :param mode: Acquisition Mode
 
         :type rate: `number`
         :param rate: Acquisition rate
 
+        :type trigger_source: `string`  ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External'] # noqa
+        :param trigger_source: Trigger source
+
+        :type trigger_level: `number` [-5V, 5V]  (defaults to 0)
+        :param trigger_level: Trigger level
+
+
         """
         super().start_streaming()
         operation = "start_streaming"
         params = dict(
             duration=duration,
             mode=validate_range(
                 mode, ['Normal', 'Precision', 'DeepMemory', 'PeakDetect']),
             rate=rate,
+            trigger_source=trigger_source,
+            trigger_level=trigger_level
         )
 
         response = self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
         self.stream_id = response["stream_id"]
```

### Comparing `moku-3.1.1/moku/instruments/_lockinamp.py` & `moku-3.2.0/moku/instruments/_lockinamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -582,15 +582,15 @@
 
         :type noise_reject: `boolean`
         :param noise_reject: Configure the Oscilloscope with a small amount of hysteresis to prevent repeated triggering due to noise # noqa
 
         :type hf_reject: `boolean`
         :param hf_reject: Configure the trigger signal to pass through a low pass filter to smooths out the noise # noqa
 
-        :type source: `string` ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD']
+        :type source: `string` ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External']
         :param source: Trigger Source
 
         """
         operation = "set_trigger"
         params = dict(
             strict=strict,
             type=validate_range(type, ['Edge', 'Pulse']),
@@ -604,15 +604,15 @@
             nth_event=nth_event,
             holdoff=holdoff,
             hysteresis=hysteresis,
             auto_sensitivity=auto_sensitivity,
             noise_reject=noise_reject,
             hf_reject=hf_reject,
             source=validate_range(
-                source, ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD']),
+                source, ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External']),
         )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
 
     def set_timebase(self, t1, t2, strict=True):
@@ -793,14 +793,16 @@
 
     def start_logging(
             self,
             duration=60,
             delay=0,
             file_name_prefix="",
             comments="",
+            trigger_source=None,
+            trigger_level=None,
             mode="Normal",
             rate=1000,
             strict=True):
         """
         start_logging.
 
         :type strict: `boolean`
@@ -808,14 +810,20 @@
 
         :type duration: `integer` Sec (defaults to 60)
         :param duration: Duration to log for
 
         :type delay: `integer` Sec (defaults to 0)
         :param delay: Delay the start by
 
+        :type trigger_source: `string`  ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External'] # noqa
+        :param trigger_source: Trigger source
+
+        :type trigger_level: `number` [-5V, 5V]  (defaults to 0)
+        :param trigger_level: Trigger level
+
         :type file_name_prefix: `string`
         :param file_name_prefix: Optional file name prefix
 
         :type comments: `string`
         :param comments: Optional comments to be included
 
         :type mode: `string` ['Normal', 'Precision', 'DeepMemory', 'PeakDetect'] # noqa
@@ -826,14 +834,16 @@
 
         """
         operation = "start_logging"
         params = dict(
             strict=strict,
             duration=duration,
             delay=delay,
+            trigger_source=trigger_source,
+            trigger_level=trigger_level,
             file_name_prefix=file_name_prefix,
             comments=comments,
             mode=validate_range(
                 mode, ['Normal', 'Precision', 'DeepMemory', 'PeakDetect']),
             rate=rate,
         )
         return self.session.post(
@@ -845,35 +855,46 @@
         """
         stop_logging.
         """
         operation = "stop_logging"
         return self.session.get(
             f"slot{self.slot}/{self.operation_group}", operation)
 
-    def start_streaming(self, duration=None, mode="Normal", rate=1000):
+    def start_streaming(self, duration=None, mode="Normal", rate=1000,
+                        trigger_source=None,
+                        trigger_level=None):
         """
         start_streaming.
 
         :type duration: `integer`
         :param duration: Duration in second(s) to stream for
 
         :type mode: `string` ['Normal', 'Precision', 'DeepMemory', 'PeakDetect'] # noqa
         :param mode: Acquisition Mode
 
         :type rate: `number`
         :param rate: Acquisition rate
 
+        :type trigger_source: `string`  ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External'] # noqa
+        :param trigger_source: Trigger source
+
+        :type trigger_level: `number` [-5V, 5V]  (defaults to 0)
+        :param trigger_level: Trigger level
+
+
         """
         super().start_streaming()
         operation = "start_streaming"
         params = dict(
             duration=duration,
             mode=validate_range(
                 mode, ['Normal', 'Precision', 'DeepMemory', 'PeakDetect']),
             rate=rate,
+            trigger_source=trigger_source,
+            trigger_level=trigger_level
         )
 
         response = self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
         self.stream_id = response["stream_id"]
```

### Comparing `moku-3.1.1/moku/instruments/_logicanalyzer.py` & `moku-3.2.0/moku/instruments/_logicanalyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
 
         """
         operation = "set_source"
         params = dict(
-            source=validate_range(source, ['DigitalIO', 'AnalogInputs', 'SlotInput']), # noqa
+            source=validate_range(source, ['DigitalIO', 'AnalogInputs', 'SlotInput']),  # noqa
             strict=strict,
         )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
 
@@ -513,15 +513,15 @@
         """
         get_timebase.
         """
         operation = "get_timebase"
         return self.session.get(
             f"slot{self.slot}/{self.operation_group}", operation)
 
-    def get_data(self, timeout=60, wait_reacquire=False, wait_complete=False, include_pins=None): # noqa
+    def get_data(self, timeout=60, wait_reacquire=False, wait_complete=False, include_pins=None):  # noqa
         """
         get_data.
 
         :type timeout: `number` Seconds (defaults to 60)
         :param timeout: Wait for n seconds to receive a data frame
 
         :type wait_reacquire: `boolean`
@@ -834,14 +834,92 @@
             spi_cpha=spi_cpha,
         )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
 
+    def set_can_decoder(
+            self,
+            channel,
+            data_bit,
+            baud_rate=500000,
+            lsb_first=False,
+            strict=True):
+        """
+        set_can_decoder.
+
+        :type strict: `boolean`
+        :param strict: Disable all implicit conversions and coercions.
+
+        :type channel: `integer`
+        :param channel: Target decoder channel
+
+        :type data_bit: `integer` [1, 16]
+        :param data_bit: Bit index to receive(Rx) signal
+
+        :type baud_rate: `integer` 500000
+        :param baud_rate: Baud Rate
+
+        :type lsb_first: `boolean`
+        :param lsb_first: Bit order. Defaults to false, making it msb_first
+
+        """
+        operation = "set_can_decoder"
+        params = dict(
+            strict=strict,
+            channel=channel,
+            data_bit=data_bit,
+            baud_rate=baud_rate,
+            lsb_first=lsb_first,
+        )
+        return self.session.post(
+            f"slot{self.slot}/{self.operation_group}",
+            operation,
+            params)
+
+    def set_parallel_bus_decoder(
+            self,
+            channel,
+            sample_mode,
+            data_width,
+            clock_bit,
+            strict=True):
+        """
+        set_parallel_bus_decoder.
+
+        :type strict: `boolean`
+        :param strict: Disable all implicit conversions and coercions.
+
+        :type channel: `integer`
+        :param channel: Target decoder channel
+
+        :type sample_mode: `string` ["Rising","Falling","Both"]
+        :param sample_mode: Sample mode
+
+        :type data_width: `integer`
+        :param data_width: Number of data bits
+
+        :type clock_bit: `boolean`
+        :param clock_bit: Clock bit.
+
+        """
+        operation = "set_parallel_bus_decoder"
+        params = dict(
+            strict=strict,
+            channel=channel,
+            sample_mode=sample_mode,
+            data_width=data_width,
+            clock_bit=clock_bit,
+        )
+        return self.session.post(
+            f"slot{self.slot}/{self.operation_group}",
+            operation,
+            params)
+
     def get_decoder(self, channel):
         """
         get_decoder.
 
         :type channel: `integer`
         :param channel: Target channel
```

### Comparing `moku-3.1.1/moku/instruments/_mim.py` & `moku-3.2.0/moku/instruments/_mim.py`

 * *Files identical despite different names*

### Comparing `moku-3.1.1/moku/instruments/_oscilloscope.py` & `moku-3.2.0/moku/instruments/_oscilloscope.py`

 * *Files identical despite different names*

### Comparing `moku-3.1.1/moku/instruments/_phasemeter.py` & `moku-3.2.0/moku/instruments/_phasemeter.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         params = dict(
             strict=strict, channel=channel, impedance=validate_range(
                 impedance, [
                     '1MOhm', '50Ohm']), coupling=validate_range(
                 coupling, [
                     'AC', 'DC']), range=validate_range(
                         range, [
-                            'Default', '400mVpp', '1Vpp', '4Vpp', '10Vpp', '40Vpp', '50Vpp']), ) # noqa
+                            'Default', '400mVpp', '1Vpp', '4Vpp', '10Vpp', '40Vpp', '50Vpp']), )  # noqa
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
 
     def get_frontend(self, channel):
         """
@@ -285,15 +285,15 @@
         :param scaling: Scaling for phase, frequency offset and amplitude
 
         """
         operation = "generate_output"
         params = dict(
             strict=strict,
             channel=channel,
-            signal=validate_range(signal, ['Sine', 'Phase', 'FrequencyOffset', 'Amplitude']), # noqa
+            signal=validate_range(signal, ['Sine', 'Phase', 'FrequencyOffset', 'Amplitude']),  # noqa
             amplitude=amplitude,
             frequency=frequency,
             frequency_multiplier=frequency_multiplier,
             phase=phase,
             offset=offset,
             phase_locked=phase_locked,
             scaling=scaling,
@@ -330,28 +330,73 @@
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
 
     def disable_input(self, channel):
         """
+        .. deprecated:: 3.1.1
+        Use `enable_input` instead.
+
         disable_input.
 
         :type channel: `integer`
         :param channel: Target channel
 
         """
         operation = "disable_input"
         params = dict(
             channel=channel,
         )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
+
+    def enable_input(self, channel, enable=True, strict=True):
+        """
+        enable_input.
+
+        :type strict: `boolean`
+        :param strict: Disable all implicit conversions and coercions.
+
+        :type channel: `integer`
+        :param channel: Target channel
+
+        :type enable: `boolean`
+        :param enable: Enable input signal
+
+        """
+        operation = "enable_input"
+        params = dict(
+            strict=strict,
+            channel=channel,
+            enable=enable,
+        )
+        return self.session.post(
+            f"slot{self.slot}/{self.operation_group}",
+            operation,
+            params)
+
+    def zero_phase(self, channel):
+        """
+        zero_phase.
+
+        :type channel: `integer`
+        :param channel: Target channel
+
+        """
+        operation = "zero_phase"
+        params = dict(
+            channel=channel,
+        )
+        return self.session.post(
+            f"slot{self.slot}/{self.operation_group}",
+            operation,
+            params)
 
     def enable_freewheeling(self, enable=True, strict=True):
         """
         enable_freewheeling.
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
```

### Comparing `moku-3.1.1/moku/instruments/_pidcontroller.py` & `moku-3.2.0/moku/instruments/_pidcontroller.py`

 * *Files 8% similar despite different names*

```diff
@@ -552,15 +552,15 @@
 
         :type noise_reject: `boolean`
         :param noise_reject: Configure the Oscilloscope with a small amount of hysteresis to prevent repeated triggering due to noise # noqa
 
         :type hf_reject: `boolean`
         :param hf_reject: Configure the trigger signal to pass through a low pass filter to smooths out the noise # noqa
 
-        :type source: `string` ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD']
+        :type source: `string` ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External']
         :param source: Trigger Source
 
         """
         operation = "set_trigger"
         params = dict(
             strict=strict,
             type=validate_range(type, ['Edge', 'Pulse']),
@@ -574,15 +574,15 @@
             nth_event=nth_event,
             holdoff=holdoff,
             hysteresis=hysteresis,
             auto_sensitivity=auto_sensitivity,
             noise_reject=noise_reject,
             hf_reject=hf_reject,
             source=validate_range(
-                source, ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD']),
+                source, ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External']),
         )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
 
     def get_frontend(self, channel):
@@ -891,14 +891,16 @@
 
     def start_logging(
             self,
             duration=60,
             delay=0,
             file_name_prefix="",
             comments="",
+            trigger_source=None,
+            trigger_level=None,
             mode="Normal",
             rate=1000,
             strict=True):
         """
         start_logging.
 
         :type strict: `boolean`
@@ -906,14 +908,20 @@
 
         :type duration: `integer` Sec (defaults to 60)
         :param duration: Duration to log for
 
         :type delay: `integer` Sec (defaults to 0)
         :param delay: Delay the start by
 
+        :type trigger_source: `string`  ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External'] # noqa
+        :param trigger_source: Trigger source
+
+        :type trigger_level: `number` [-5V, 5V]  (defaults to 0)
+        :param trigger_level: Trigger level
+
         :type file_name_prefix: `string`
         :param file_name_prefix: Optional file name prefix
 
         :type comments: `string`
         :param comments: Optional comments to be included
 
         :type mode: `string` ['Normal', 'Precision', 'DeepMemory', 'PeakDetect'] # noqa
@@ -924,14 +932,16 @@
 
         """
         operation = "start_logging"
         params = dict(
             strict=strict,
             duration=duration,
             delay=delay,
+            trigger_source=trigger_source,
+            trigger_level=trigger_level,
             file_name_prefix=file_name_prefix,
             comments=comments,
             mode=validate_range(
                 mode, ['Normal', 'Precision', 'DeepMemory', 'PeakDetect']),
             rate=rate,
         )
         return self.session.post(
@@ -943,35 +953,46 @@
         """
         stop_logging.
         """
         operation = "stop_logging"
         return self.session.get(
             f"slot{self.slot}/{self.operation_group}", operation)
 
-    def start_streaming(self, duration=None, mode="Normal", rate=1000):
+    def start_streaming(self, duration=None, mode="Normal", rate=1000,
+                        trigger_source=None,
+                        trigger_level=None):
         """
         start_streaming.
 
         :type duration: `integer`
         :param duration: Duration in second(s) to stream for
 
         :type mode: `string` ['Normal', 'Precision', 'DeepMemory', 'PeakDetect'] # noqa
         :param mode: Acquisition Mode
 
         :type rate: `number`
         :param rate: Acquisition rate
 
+        :type trigger_source: `string`  ['ProbeA', 'ProbeB', 'ProbeC', 'ProbeD', 'External'] # noqa
+        :param trigger_source: Trigger source
+
+        :type trigger_level: `number` [-5V, 5V]  (defaults to 0)
+        :param trigger_level: Trigger level
+
+
         """
         super().start_streaming()
         operation = "start_streaming"
         params = dict(
             duration=duration,
             mode=validate_range(
                 mode, ['Normal', 'Precision', 'DeepMemory', 'PeakDetect']),
             rate=rate,
+            trigger_source=trigger_source,
+            trigger_level=trigger_level
         )
         response = self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
         self.stream_id = response["stream_id"]
         self.ip_address = self.session.ip_address
```

### Comparing `moku-3.1.1/moku/instruments/_spectrumanalyzer.py` & `moku-3.2.0/moku/instruments/_spectrumanalyzer.py`

 * *Files 13% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         params = dict(
             strict=strict, channel=channel, impedance=validate_range(
                 impedance, [
                     '1MOhm', '50Ohm']), coupling=validate_range(
                 coupling, [
                     'AC', 'DC']), range=validate_range(
                         range, [
-                            'Default', '400mVpp', '1Vpp', '4Vpp', '10Vpp', '40Vpp', '50Vpp']), ) # noqa
+                            'Default', '400mVpp', '1Vpp', '4Vpp', '10Vpp', '40Vpp', '50Vpp']), )  # noqa
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
 
     def get_frontend(self, channel):
         """
@@ -113,15 +113,15 @@
 
         """
         operation = "get_frontend"
         params = dict(
             channel=channel,
         )
         return self.session.post(
-            f"slot{self.slot}/{self.operation_group}", operation, params=params) # noqa
+            f"slot{self.slot}/{self.operation_group}", operation, params=params)  # noqa
 
     def sa_output(self, channel, amplitude, frequency, strict=True):
         """
         sa_output.
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
@@ -370,14 +370,69 @@
             channel=channel,
         )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
 
+    def set_averaging(self, target_duration=0.1, strict=True):
+        """
+        set_averaging
+
+        :type target_duration: `boolean`
+        :param target_duration: Average frames for the given duration.
+
+        :type strict: `boolean`
+        :param strict: Disable all implicit conversions and coercions.
+
+        """
+        operation = "set_averaging"
+        params = dict(
+            target_duration=target_duration,
+            strict=strict
+        )
+        return self.session.post(
+            f"slot{self.slot}/{self.operation_group}",
+            operation,
+            params)
+
+    def enable_xcorr(self, channel_a, channel_b, strict=True):
+        """
+        enable_xcorr
+
+        :type channel_a: `string` ['Input1', 'Input2', 'Input3', 'Input4', 'InputA', 'InputB', 'InputC', 'InputD'] # noqa
+        :param channel_a: First channel to cross correlate
+
+        :type channel_b: `string` ['Input1', 'Input2', 'Input3', 'Input4', 'InputA', 'InputB', 'InputC', 'InputD'] # noqa
+        :param channel_b: Second channel to cross correlate
+
+        :type strict: `boolean`
+        :param strict: Disable all implicit conversions and coercions.
+
+        """
+        operation = "enable_xcorr"
+        params = dict(
+            channel_a=channel_a,
+            channel_b=channel_b,
+            strict=strict
+        )
+        return self.session.post(
+            f"slot{self.slot}/{self.operation_group}",
+            operation,
+            params)
+
+    def disable_xcorr(self):
+        """
+        disable_xcorr
+        """
+        operation = "disable_xcorr"
+        return self.session.post(
+            f"slot{self.slot}/{self.operation_group}",
+            operation)
+
     def get_data(
             self,
             timeout=60,
             wait_reacquire=False,
             wait_complete=True,
             units="dBm",
             psdUnits=False,
```

### Comparing `moku-3.1.1/moku/instruments/_stream.py` & `moku-3.2.0/moku/instruments/_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 from threading import Event, Thread
 
 from moku import MOKU_CLI_PATH
 from moku.utilities import check_mokucli_version
 from moku.exceptions import StreamException
 
 moku_cli_streaming_compat = {
-    # fw_ver: (cli_major_version, cli_minor_version, cli_patch_version) 
+    # fw_ver: (cli_major_version, cli_minor_version, cli_patch_version)
     580: (2, 1, 0),
     585: (2, 2, 1),
+    590: (2, 2, 2),
 }
 
+
 class MokuCLIThread(Thread):
     """
     Threadinng class responsible to run the mokucli command.
 
     :param command: Command to execute as a subprocess
     :param start_evt: Event object to set once the subprocess is launched
     """
@@ -51,24 +53,32 @@
     def __init__(self, firmware_version):
         self.stream_id = None
         self.ip_address = None
         self.port = None
         self._socket_rdr = None
         self._running = False
         self._error_event = Event()
-        self._compat_cli_ver = self._get_compatible_cli_version(firmware_version)
+        self._compat_cli_ver = self._get_compatible_cli_version(firmware_version)  # noqa
 
     @staticmethod
     def _get_next_available_port():
         sock = socket.socket()
         sock.bind(('', 0))
         port = sock.getsockname()[1]
         sock.close()
         return port
 
+    def _reset_stream_config(self):
+        self.stream_id = None
+        self.ip_address = None
+        self.port = None
+        self._socket_rdr = None
+        self._running = False
+        self._error_event = Event()
+
     def _get_compatible_cli_version(self, firmware_version):
         versions = list(moku_cli_streaming_compat.keys())
         if firmware_version in versions:
             return moku_cli_streaming_compat[firmware_version]
         # default to latest version
         return moku_cli_streaming_compat[max(versions)]
 
@@ -102,27 +112,30 @@
         cli_thread = MokuCLIThread(command, self._error_event, _start_event)
         cli_thread.start()
         _start_event.wait()
         self._running = True
         self._connect()
 
     def start_streaming(self):
+        """
+        Base class start_streaming, verifies if streaming is possible
+        """
         check_mokucli_version(MOKU_CLI_PATH, self._compat_cli_ver)
 
     def stream_to_file(self, name=None):
         """
         Streams the data to the file of desired format
 
         :type name: `string`
         :param name: Base name with one of csv, npy, mat extensions (defaults to csv) # noqa
 
         """
         if not self.stream_id:
             raise StreamException(
-                "No streaming session in progress, start one using start_streaming") # noqa
+                "No streaming session in progress, start one using start_streaming")  # noqa
         if not self._running:
             check_mokucli_version(MOKU_CLI_PATH, self._compat_cli_ver)
             _ip = f"--ip-address={self.ip_address}"
             _stream = f"--stream-id={self.stream_id}"
 
             if not name:
                 _ts = datetime.now()
@@ -137,18 +150,19 @@
         """
         Get the converted stream of data
 
         :raises StreamException: Indicates END OF STREAM
         """
         if not self.stream_id:
             raise StreamException(
-                "No streaming session in progress, start one using start_streaming") # noqa
+                "No streaming session in progress, start one using start_streaming")  # noqa
         if self._error_event.is_set():
             raise Exception
         if not self._running:
             check_mokucli_version(MOKU_CLI_PATH, self._compat_cli_ver)
             self._begin_streaming()
         data = self._socket_rdr.readline()
         if data:
             if data == "EOS\n":
+                self._reset_stream_config()
                 raise StreamException("End of stream")
             return json.loads(data)
```

### Comparing `moku-3.1.1/moku/instruments/_waveformgenerator.py` & `moku-3.2.0/moku/instruments/_waveformgenerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
 
         :type channel: `integer`
         :param channel: Target channel
 
         :type type: `string` ['Amplitude', 'Frequency', 'Phase', 'PulseWidth']
         :param type: Modulation type
 
-        :type source: `string` ['Input1', 'Input2', 'Input3', 'Input4', 'InputA', 'InputB', 'InputC', 'InputD', 'Output1', 'Output2', 'Output3', 'Output4', 'Internal'] # noqa
+        :type source: `string` ['Input1', 'Input2', 'Input3', 'Input4', 'InputA', 'InputB', 'InputC', 'InputD', 'Output1', 'Output2', 'Output3', 'Output4', 'OutputA', 'OutputB', 'Internal'] # noqa
         :param source: Modulation source
 
         :type depth: `number`  (defaults to 0)
         :param depth: Modulation depth (depends on modulation type): Percentage modulation depth, Frequency Deviation/Volt or +/- phase shift/Volt # noqa
 
         :type frequency: `number` [0Hz, 50e6Hz]  (defaults to 10000000)
         :param frequency: Frequency of internally-generated sine wave modulation. This parameter is ignored if the source is set to ADC or DAC. # noqa
@@ -305,14 +305,16 @@
                                              'InputB',
                                              'InputC',
                                              'InputD',
                                              'Output1',
                                              'Output2',
                                              'Output3',
                                              'Output4',
+                                             'OutputA',
+                                             'OutputB',
                                              'Internal']),
                       depth=depth,
                       frequency=frequency,
                       )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
```

### Comparing `moku-3.1.1/moku/session.py` & `moku-3.2.0/moku/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,38 @@
 
 from requests import Session
 
 from . import exceptions
 
 
 def handle_response(func):
+    """
+    Decorator which parses the response returned
+    by Moku API Server
+    """
     @wraps(func)
     def func_wrapper(self, *args, **kwargs):
         response = func(self, *args, **kwargs)
         return self.resolve(response)
 
     return func_wrapper
 
 
 class RequestSession:
+    "Base HTTP Requests class"
     json_headers = {'Content-type': 'application/json'}
     sk_name = "Moku-Client-Key"  # session key name
 
     def __init__(self, ip, connect_timeout, read_timeout, **kwargs):
         self.ip_address = ip
         self.connect_timeout = connect_timeout
         self.read_timeout = read_timeout
-        self.session_key = None
         self.rs = Session()
+
+        # support arbitrary session arguments
         for k, v in kwargs.items():
             if k.lower().startswith("session_"):
                 k = k.split("session_")[1]
                 setattr(self.rs, k, v)
 
     def update_sk(self, response):
         key = response.headers.get(self.sk_name)
@@ -40,37 +46,41 @@
     def url_for(self, group, operation):
         return f'http://{self.ip_address}/api/{group}/{operation}'
 
     def url_for_v2(self, location):
         return f'http://{self.ip_address}/api/v2/{location}'
 
     def timeout_headers(self, rt_increase=0):
+        "Returns timeout headers required for http request"
         return tuple([self.connect_timeout,
                       self.read_timeout + rt_increase])
 
     @handle_response
     def get(self, group, operation):
+        "Executes get call and returns the response"
         return self.rs.get(self.url_for(group, operation),
                            timeout=self.timeout_headers())
 
     @handle_response
     def post(self, group, operation, params=None):
+        "Executes post call and returns the response"
         # As get_data has an explicit read_timeout parameter,
         # it should be considered applicable cases, in all other
         # cases default it to 0
         _timeout = None
         if params:
             _timeout = params.get('timeout', 0)
         _to_inc = 0 if not _timeout else _timeout
         return self.rs.post(self.url_for(group, operation),
                             json=params,
                             timeout=self.timeout_headers(_to_inc),
                             headers=self.json_headers)
 
     def post_to_v2_raw(self, location, params=None):
+        "Executes post call to api v2 and returns the response"
         response = self.rs.post(self.url_for_v2(location),
                                 json=params)
         return response
 
     def post_to_v2(self, location, params=None):
         response = self.rs.post(self.url_for_v2(location),
                                 json=params)
@@ -90,33 +100,20 @@
     @handle_response
     def post_file(self, group, operation, data):
         return self.rs.post(self.url_for(group, operation),
                             data=data, timeout=self.timeout_headers())
 
     @handle_response
     def delete_file(self, group, operation):
+        "Deletes the given file from the Moku"
         return self.rs.delete(self.url_for(group, operation),
                               timeout=self.timeout_headers())
 
     @staticmethod
-    def handle_http_error(response):
-        if response.status_code == 500:
-            raise exceptions.MokuException(
-                "Unhandled error received from Moku.")
-        if response.status_code == 404:
-            raise exceptions.OperationNotFound(
-                "Method not found. Make sure Python Client "
-                "is compatible with the firmware version running")
-        else:
-            raise exceptions.MokuException(
-                f"Unknown exception. "
-                f"Status code:{response.status_code}")
-
-    @staticmethod
-    def handle_error(code, messages):
+    def _handle_error(code, messages):
         if code == "NO_PLATFORM_BIT_STREAM":
             raise exceptions.NoPlatformBitstream(messages)
         elif code == "NO_BIT_STREAM":
             raise exceptions.NoInstrumentBitstream(messages)
         elif code == "INVALID_PARAM":
             raise exceptions.InvalidParameterException(messages)
         elif code == "INVALID_REQUEST":
@@ -126,14 +123,15 @@
         elif code == "UNEXPECTED_CHANGE":
             raise exceptions.UnexpectedChangeError(messages)
         else:
             raise exceptions.MokuException(messages)
 
     @staticmethod
     def echo_warnings(messages):
+        "Prints any warnings received from Moku"
         for m in messages or []:
             print(f"Warning: {m}")
 
     @staticmethod
     def _normalize_nan_inf(arg):
         return {"-inf": -float("inf"),
                 "inf": float("inf"),
@@ -145,25 +143,35 @@
         except json.decoder.JSONDecodeError:
             content = content.replace('nan', '"nan"')
             content = content.replace('inf', '"inf"')
             return json.loads(content,
                               parse_constant=self._normalize_nan_inf)
 
     def resolve(self, response):
+        "Resolves response received"
         def _parse_to_object(content):
             content = content.decode("utf-8")
             content = self._check_and_normalize_nan_inf(content)
             return namedtuple("_", content.keys())(*content.values())
 
-        self.update_sk(response)
-        if response is not None:
-            if response.status_code == 200:
-                data = _parse_to_object(response.content)
-                if data.success is True:
-                    self.echo_warnings(data.messages)
-                    return data.data
-                elif data.success is False:
-                    self.handle_error(data.code, data.messages)
-            else:
-                self.handle_http_error(response)
+        key = response.headers.get(self.sk_name)
+        if key:
+            self.rs.headers.update({self.sk_name: key})
+        if response.status_code == 200:
+            data = _parse_to_object(response.content)
+            if data.success is True:
+                self.echo_warnings(data.messages)
+                return data.data
+            elif data.success is False:
+                self._handle_error(data.code, data.messages)
         else:
-            raise Exception('Response object empty')
+            print(response.__dict__)
+            if response.status_code == 500:
+                raise exceptions.MokuException(
+                    "Unhandled error received from Moku.")
+            if response.status_code == 404:
+                raise exceptions.OperationNotFound(
+                    "Method not found. Make sure Python Client is compatible with the firmware version running")  # noqa
+            else:
+                raise exceptions.MokuException(
+                    f"Unknown exception. "
+                    f"Status code:{response.status_code}")
```

### Comparing `moku-3.1.1/moku/utilities.py` & `moku-3.2.0/moku/utilities.py`

 * *Files identical despite different names*

### Comparing `moku-3.1.1/moku.egg-info/PKG-INFO` & `moku-3.2.0/moku.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moku
-Version: 3.1.1
+Version: 3.2.0
 Summary: Python scripting interface to the Liquid Instruments Moku hardware
 Home-page: https://liquidinstruments.com
 Author: Liquid Instruments
 Author-email: info@liquidinstruments.com
 License: MIT
 Description: 
                 # Moku
```

### Comparing `moku-3.1.1/moku.egg-info/SOURCES.txt` & `moku-3.2.0/moku.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+LICENSE.txt
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 moku/__init__.py
 moku/cli.py
 moku/exceptions.py
 moku/finder.py
 moku/session.py
@@ -27,8 +29,11 @@
 moku/instruments/_logicanalyzer.py
 moku/instruments/_mim.py
 moku/instruments/_oscilloscope.py
 moku/instruments/_phasemeter.py
 moku/instruments/_pidcontroller.py
 moku/instruments/_spectrumanalyzer.py
 moku/instruments/_stream.py
-moku/instruments/_waveformgenerator.py
+moku/instruments/_tfa.py
+moku/instruments/_waveformgenerator.py
+tests/test(2).py
+tests/test_dl.py
```

### Comparing `moku-3.1.1/setup.py` & `moku-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 import os.path
 
 setup(
     name="moku",
-    version="3.1.1",
+    version="3.2.0",
     author='Liquid Instruments',
     author_email='info@liquidinstruments.com',
     packages=['moku'],
     package_dir={'moku': 'moku'},
     package_data={
         'moku': [
             os.path.join('instruments', '*'),
```

