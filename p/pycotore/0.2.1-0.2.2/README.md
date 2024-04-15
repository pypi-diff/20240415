# Comparing `tmp/pycotore-0.2.1.tar.gz` & `tmp/pycotore-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycotore-0.2.1.tar", max compression
+gzip compressed data, was "pycotore-0.2.2.tar", max compression
```

## Comparing `pycotore-0.2.1.tar` & `pycotore-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.2.1/LICENSE
--rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.2.1/README.md
--rw-r--r--   0        0        0      124 2024-04-12 06:18:55.434725 pycotore-0.2.1/pycotore/__init__.py
--rw-r--r--   0        0        0      398 2024-04-11 13:49:12.930662 pycotore-0.2.1/pycotore/converter.py
--rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.2.1/pycotore/exceptions.py
--rw-r--r--   0        0        0     2049 2024-04-12 06:35:18.485819 pycotore-0.2.1/pycotore/logger.py
--rw-r--r--   0        0        0     6671 2024-04-12 06:22:19.124560 pycotore-0.2.1/pycotore/progress.py
--rw-r--r--   0        0        0      597 2024-04-12 06:35:28.362825 pycotore-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.2.2/LICENSE
+-rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.2.2/README.md
+-rw-r--r--   0        0        0      124 2024-04-12 06:18:55.434725 pycotore-0.2.2/pycotore/__init__.py
+-rw-r--r--   0        0        0      398 2024-04-11 13:49:12.930662 pycotore-0.2.2/pycotore/converter.py
+-rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.2.2/pycotore/exceptions.py
+-rw-r--r--   0        0        0     2049 2024-04-12 06:35:18.485819 pycotore-0.2.2/pycotore/logger.py
+-rw-r--r--   0        0        0     7591 2024-04-12 20:14:19.492185 pycotore-0.2.2/pycotore/progress.py
+-rw-r--r--   0        0        0      597 2024-04-12 19:09:15.311572 pycotore-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.2.2/PKG-INFO
```

### Comparing `pycotore-0.2.1/LICENSE` & `pycotore-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycotore-0.2.1/pycotore/logger.py` & `pycotore-0.2.2/pycotore/logger.py`

 * *Files identical despite different names*

### Comparing `pycotore-0.2.1/pycotore/progress.py` & `pycotore-0.2.2/pycotore/progress.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,77 +13,90 @@
     show_preffix: bool = False
     show_bar: bool = True
     _speed = "[SPEED: {0: ^7.2f}{1:<3}]"
     _percents = "[{0:>6.2f}%]"
     _time_left = "[LEFT: {0:0>2}:{1:0>2}:{2:0>2}]"
     _running = "[RUN: {0:0>2}:{1:0>2}:{2:0>2}]"
     _progress = "[{:{done_marker}>{done_size}}{}{:{base_marker}>{left_size}}]"
+    _total_progress = "[{0: ^8.2f}{1:<3}]"
     _completed: float = 0.00
     current_marker: list = ["-", "\\", "|", "/"]
     filler_marker: str = " "
     bar_length: int = 0
     bar_size: int = 0
     _preffix: str = ""
     _suffix: str = ""
     _done_marker: str = "#"
-    _total = 100.00
+    _total: float = 100.00
 
     def __init__(
                 self,
                 show_percents: bool = True,
                 show_estimate: bool = True,
                 show_runtime: bool = True,
-                show_speed: bool = True
+                show_speed: bool = True,
+                show_transfer: bool = True
             ):
         self.terminal_size: int = os.get_terminal_size().columns
         self.percents: str = self._percents.format(0)
         self.show_percents: bool = show_percents
         self.show_numbers: bool = False
         self.time_start = datetime.now()
         self.show_estimate: bool = show_estimate
         self.time_left = self._time_left.format(99, 59, 59)
         self.run_time = self._running.format(0, 0, 0)
         self._run_time = datetime.now()
         self.speed = self._speed.format(0, "b")
+        self.total_progress = self._total_progress.format(0, "b")
         self.show_runtime: bool = show_runtime
+        self.show_transfer: bool = show_transfer
         self.avg_speed = 0
         self.show_speed = show_speed
 
     def __update_stats(self) -> None:
         self.__run_time()
         self.__update_avg_speed()
         if self.show_percents:
             self.__update_percent_done()
         if self.show_estimate:
             self.__calculate_estimate()
         if self.show_runtime:
             self.__update_run_time()
         if self.show_speed:
             self.__update_speed()
+        if self.show_transfer:
+            self.__total_progress()
         self.__update_terminal_size()
 
     def __get_current_marker(self) -> str:
         self.current_marker.append(self.current_marker.pop(0))
         return self.current_marker[-1]
 
     def __update_speed(self) -> None:
         speed, units = convert_to_human(self.avg_speed)
         self.speed = self._speed.format(speed, units)
 
+    def __total_progress(self) -> None:
+        progress, units = convert_to_human(self.progress)
+        self.total_progress = self._total_progress.format(progress, units)
+
     def __run_time(self) -> None:
         self._run_time = datetime.now() - self.time_start
 
     def __update_terminal_size(self) -> None:
         self.terminal_size = os.get_terminal_size().columns
 
     def __split_time(self, seconds: int) -> list:
         result = []
-        result.append(int(seconds // 3600))
-        result.append(int(seconds // 60))
-        result.append(int(seconds % 60))
+        hours = int(seconds // 3600)
+        minutes = int(seconds // 60)
+        seconds = int(seconds % 60)
+        result.append(hours if hours > 0 else 0)
+        result.append(minutes if minutes > 0 else 0)
+        result.append(seconds if minutes >= 0 else 0)
         return result
 
     def __update_run_time(self) -> None:
         time = self.__split_time(self._run_time.total_seconds())
         self.run_time = self._running.format(time[0], time[1], time[2])
 
     def __update_avg_speed(self) -> None:
@@ -105,14 +118,17 @@
     def __format_bar(self) -> str:
         bar = [""]
         bar_info = 0
         finished = int(self.bar_size * self.progress / self.total)
         if self.show_preffix:
             bar.append(self.preffix)
             bar_info += len(self.preffix)
+        if self.show_transfer:
+            bar.append(self.total_progress)
+            bar_info += len(self.total_progress)
         if self.show_bar:
             bar.append("")
             bar_index = len(bar) - 1
         if self.show_percents:
             bar.append(self.percents)
             bar_info += len(self.percents)
         if self.show_runtime:
@@ -124,26 +140,29 @@
         if self.show_speed:
             bar.append(self.speed)
             bar_info += len(self.speed)
         if self.show_suffix:
             bar.append(self.suffix)
             bar_info += len(self.suffix)
         if bar_index:
-            self.bar_size = self.terminal_size - bar_info - 3
-            left_size = self.bar_size - finished
-            bar[bar_index] = self._progress.format(
-                    self._done_marker if finished > 1 else "",
-                    self.__get_current_marker() if left_size > 0 else "",
-                    self.filler_marker if left_size > 0 else "",
-                    done_marker=self._done_marker,
-                    done_size=finished,
-                    in_progress_marker=self.filler_marker,
-                    base_marker=self.filler_marker,
-                    left_size=left_size
-                )
+            if self.terminal_size > bar_info:
+                self.bar_size = self.terminal_size - bar_info - 3
+                left_size = self.bar_size - finished
+                bar[bar_index] = self._progress.format(
+                        self._done_marker if finished > 1 else "",
+                        self.__get_current_marker() if left_size > 0 else "",
+                        self.filler_marker if left_size > 0 else "",
+                        done_marker=self._done_marker,
+                        done_size=finished if left_size > 0 else self.bar_size,
+                        in_progress_marker=self.filler_marker,
+                        base_marker=self.filler_marker,
+                        left_size=left_size if left_size > 0 else 0
+                    )
+            else:
+                bar.pop(bar_index)
         if self.bar_size <= finished:
             self.current_marker = ""
         bar.append("\r")
         line = "".join(bar)
         return line
 
     @property
```

### Comparing `pycotore-0.2.1/pyproject.toml` & `pycotore-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "pycotore"
 readme = "README.md"
 authors = ["Arunas Grigalionis <arunas.grigalionis@gmail.com>"]
 description = "Generic classes for reuse"
-version = "0.2.1"
+version = "0.2.2"
 license = "GPL-3.0-only"
 homepage = "https://github.com/niekosau"
 repository = "https://github.com/niekosau/pycotore"
 
 [tool.poetry.dependencies]
 python = "~3.9"
```

### Comparing `pycotore-0.2.1/PKG-INFO` & `pycotore-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycotore
-Version: 0.2.1
+Version: 0.2.2
 Summary: Generic classes for reuse
 Home-page: https://github.com/niekosau
 License: GPL-3.0-only
 Author: Arunas Grigalionis
 Author-email: arunas.grigalionis@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

