# Comparing `tmp/dsp_ifsc-0.0.5.tar.gz` & `tmp/dsp_ifsc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_ifsc-0.0.5.tar", max compression
+gzip compressed data, was "dsp_ifsc-0.0.6.tar", max compression
```

## Comparing `dsp_ifsc-0.0.5.tar` & `dsp_ifsc-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.5/LICENSE
--rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.5/README.md
--rw-r--r--   0        0        0        0 2024-04-14 21:18:08.641250 dsp_ifsc-0.0.5/dsp_ifsc/__init__.py
--rw-r--r--   0        0        0     2282 2024-04-14 22:03:29.782544 dsp_ifsc-0.0.5/dsp_ifsc/sequence.py
--rw-r--r--   0        0        0    11838 2024-04-14 22:41:37.958897 dsp_ifsc-0.0.5/dsp_ifsc/signal.py
--rw-r--r--   0        0        0     1007 2024-04-14 22:43:55.336954 dsp_ifsc-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.6/LICENSE
+-rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 21:18:08.641250 dsp_ifsc-0.0.6/dsp_ifsc/__init__.py
+-rw-r--r--   0        0        0     2282 2024-04-14 22:03:29.782544 dsp_ifsc-0.0.6/dsp_ifsc/sequence.py
+-rw-r--r--   0        0        0    12145 2024-04-14 23:06:15.841463 dsp_ifsc-0.0.6/dsp_ifsc/signal.py
+-rw-r--r--   0        0        0     1007 2024-04-14 23:06:27.038345 dsp_ifsc-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.6/PKG-INFO
```

### Comparing `dsp_ifsc-0.0.5/LICENSE` & `dsp_ifsc-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_ifsc-0.0.5/dsp_ifsc/sequence.py` & `dsp_ifsc-0.0.6/dsp_ifsc/sequence.py`

 * *Files identical despite different names*

### Comparing `dsp_ifsc-0.0.5/dsp_ifsc/signal.py` & `dsp_ifsc-0.0.6/dsp_ifsc/signal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Self, Optional
 # External
 import numpy
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
+from matplotlib.ticker import MaxNLocator, AutoMinorLocator
 # Signals
 import dsp_ifsc.sequence as sequence
 
 
 class Signal:
     """
     The Signal class represents a signal in the discrete domain.
@@ -188,29 +189,35 @@
 
         y = numpy.correlate(self.x, other.x)
         n = numpy.arange(self.n.min(0) - other.n.max(0), self.n.max(0) - other.n.min(0) + 1)
 
         return Signal(y, n)
 
 
-    def stem(self, plot: Optional[Axes] = None, auto_plot: Optional[bool] = True) -> Axes:
+    def stem(
+        self,
+        plot: Optional[Axes] = None,
+        auto_plot: Optional[bool] = True,
+        x_ticks: Optional[numpy.ndarray] = None,
+        y_ticks: Optional[numpy.ndarray] = None
+    ) -> Axes:
         """
         Plots the signal.
         """
 
         if plot is None:
             plot = plt.subplot()
 
         plot.stem(self.n, self.x)
         # Adjust grid and axes scales and intervals
-        plot.grid(alpha = 0.3)
-        x_ticks = numpy.round(numpy.linspace(self.n.min(), self.n.max(), 10), 2)
-        y_ticks = numpy.round(numpy.linspace(self.x.min(), self.x.max() + self.x.max() / 10, 10), 2)
-        plot.set_xticks(x_ticks)
-        plot.set_yticks(y_ticks)
+        plot.xaxis.set_major_locator(MaxNLocator(nbins = 'auto'))  # Automatically adjust x-ticks
+        plot.yaxis.set_major_locator(MaxNLocator(nbins = 'auto'))  # Automatically adjust y-ticks
+        plot.xaxis.set_minor_locator(AutoMinorLocator())
+        plot.yaxis.set_minor_locator(AutoMinorLocator())
+        plot.grid(True, which = 'both', linestyle = '--', linewidth = 0.5, alpha = 0.7)
         # Details
         plot.set_xlabel('n')
         plot.set_ylabel('x(n)')
         plot.set_title('Signal')
 
         if auto_plot:
             plt.show()
```

### Comparing `dsp_ifsc-0.0.5/pyproject.toml` & `dsp_ifsc-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project.urls]
 Homepage = "https://github.com/JoaoMario109/ifsc-dsp-2024"
 Issues = "https://github.com/JoaoMario109/ifsc-dsp-2024/issues"
 
 [tool.poetry]
 name = "dsp-ifsc"
-version = "0.0.5"
+version = "0.0.6"
 description = "A small package with some utilities for DSP grade at IFSC - Campus Florianópolis"
 authors = [
     "João Mário Lago <joao.mcil2003@aluno.ifsc.edu.br>",
     "Alejo Perdomo Milar <alejo.pm@aluno.ifsc.edu.br>"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `dsp_ifsc-0.0.5/PKG-INFO` & `dsp_ifsc-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-ifsc
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small package with some utilities for DSP grade at IFSC - Campus Florianópolis
 Home-page: https://github.com/JoaoMario109/ifsc-dsp-2024
 License: MIT
 Author: João Mário Lago
 Author-email: joao.mcil2003@aluno.ifsc.edu.br
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

