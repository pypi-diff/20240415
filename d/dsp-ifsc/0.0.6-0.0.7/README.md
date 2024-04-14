# Comparing `tmp/dsp_ifsc-0.0.6.tar.gz` & `tmp/dsp_ifsc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_ifsc-0.0.6.tar", max compression
+gzip compressed data, was "dsp_ifsc-0.0.7.tar", max compression
```

## Comparing `dsp_ifsc-0.0.6.tar` & `dsp_ifsc-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.6/LICENSE
--rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.6/README.md
--rw-r--r--   0        0        0        0 2024-04-14 21:18:08.641250 dsp_ifsc-0.0.6/dsp_ifsc/__init__.py
--rw-r--r--   0        0        0     2282 2024-04-14 22:03:29.782544 dsp_ifsc-0.0.6/dsp_ifsc/sequence.py
--rw-r--r--   0        0        0    12145 2024-04-14 23:06:15.841463 dsp_ifsc-0.0.6/dsp_ifsc/signal.py
--rw-r--r--   0        0        0     1007 2024-04-14 23:06:27.038345 dsp_ifsc-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.7/LICENSE
+-rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 21:18:08.641250 dsp_ifsc-0.0.7/dsp_ifsc/__init__.py
+-rw-r--r--   0        0        0     2281 2024-04-14 23:21:14.820331 dsp_ifsc-0.0.7/dsp_ifsc/sequence.py
+-rw-r--r--   0        0        0    12337 2024-04-14 23:22:16.931388 dsp_ifsc-0.0.7/dsp_ifsc/signal.py
+-rw-r--r--   0        0        0     1007 2024-04-14 23:22:39.458439 dsp_ifsc-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.7/PKG-INFO
```

### Comparing `dsp_ifsc-0.0.6/LICENSE` & `dsp_ifsc-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_ifsc-0.0.6/dsp_ifsc/sequence.py` & `dsp_ifsc-0.0.7/dsp_ifsc/sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     n = numpy.arange(n_start, n_end + 1)
     x = (n - position) * slope
 
     return x, n
 
 
-def exponential(amplitude: float, decay: float, position: int, n_start: int, n_end: int) -> Tuple[numpy.ndarray, numpy.ndarray]:
+def exponential(amplitude: float, alpha: float, position: int, n_start: int, n_end: int) -> Tuple[numpy.ndarray, numpy.ndarray]:
     """
     Generates x(n) = a * exp(-b * (n - n0)); n_start <= n <= n_end
     Args:
         amplitude: The amplitude of the exponential.
         decay: The decay of the exponential.
         position: The position of the exponential.
         n_start: The start of the sequence.
@@ -72,10 +72,10 @@
 
     Returns:
         x: The exponential sequence.
         n: The sequence of n values from n_start to n_end.
     """
 
     n = numpy.arange(n_start, n_end + 1)
-    x = amplitude * numpy.exp(-decay * (n - position))
+    x = amplitude * numpy.exp(alpha * (n - position))
 
     return x, n
```

### Comparing `dsp_ifsc-0.0.6/dsp_ifsc/signal.py` & `dsp_ifsc-0.0.7/dsp_ifsc/signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,21 +189,15 @@
 
         y = numpy.correlate(self.x, other.x)
         n = numpy.arange(self.n.min(0) - other.n.max(0), self.n.max(0) - other.n.min(0) + 1)
 
         return Signal(y, n)
 
 
-    def stem(
-        self,
-        plot: Optional[Axes] = None,
-        auto_plot: Optional[bool] = True,
-        x_ticks: Optional[numpy.ndarray] = None,
-        y_ticks: Optional[numpy.ndarray] = None
-    ) -> Axes:
+    def stem(self, plot: Optional[Axes] = None, auto_plot: Optional[bool] = True) -> Axes:
         """
         Plots the signal.
         """
 
         if plot is None:
             plot = plt.subplot()
 
@@ -452,14 +446,29 @@
         """
 
         return other.correlation(self)
 
 
     # Static methods
 
+    @staticmethod
+    def from_zeros(n: numpy.ndarray) -> 'Signal':
+        """
+        Generates a zero signal.
+        Args:
+            n: The sequence of n values.
+
+        Returns:
+            signal: The zero Signal class.
+        """
+
+        x = numpy.zeros(len(n))
+
+        return Signal(x, n)
+
 
     @staticmethod
     def from_scalar(scalar: float, n: numpy.ndarray) -> 'Signal':
         """
         Generates a scalar signal.
         Args:
             scalar: The scalar value.
@@ -471,15 +480,15 @@
 
         x = scalar * numpy.ones(len(n))
 
         return Signal(x, n)
 
 
     @staticmethod
-    def from_impulse(position: int, n: numpy.ndarray) -> 'Signal':
+    def from_impulse(n: numpy.ndarray, position: int = 0) -> 'Signal':
         """
         Generates an impulse signal.
         Args:
             position: The position of the impulse.
             n: The sequence of n values.
 
         Returns:
@@ -488,43 +497,43 @@
 
         x, _n = sequence.impulse(position, n.min(), n.max())
 
         return Signal(x, _n)
 
 
     @staticmethod
-    def from_step(position: int, n: numpy.ndarray):
+    def from_step(n: numpy.ndarray, position: int = 0):
         """
         Generates a step signal.
         Returns:
             signal: The step Signal class.
         """
 
         x, _n = sequence.step(position, n.min(), n.max())
 
         return Signal(x, _n)
 
 
     @staticmethod
-    def from_ramp(slope: float, position: int, n: numpy.ndarray):
+    def from_ramp(slope: float, n: numpy.ndarray, position: int = 0):
         """
         Generates a ramp signal.
         Returns:
             signal: The ramp Signal class.
         """
 
         x, _n = sequence.ramp(slope, position, n.min(), n.max())
 
         return Signal(x, _n)
 
 
     @staticmethod
-    def from_exponential(amplitude: float, decay: float, position: int, n: numpy.ndarray):
+    def from_exponential(amplitude: float, alpha: float, n: numpy.ndarray, position: int = 0):
         """
         Generates an exponential signal.
         Returns:
             signal: The exponential Signal class.
         """
 
-        x, _n = sequence.exponential(amplitude, decay, position, n.min(), n.max())
+        x, _n = sequence.exponential(amplitude, alpha, position, n.min(), n.max())
 
         return Signal(x, _n)
```

### Comparing `dsp_ifsc-0.0.6/pyproject.toml` & `dsp_ifsc-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project.urls]
 Homepage = "https://github.com/JoaoMario109/ifsc-dsp-2024"
 Issues = "https://github.com/JoaoMario109/ifsc-dsp-2024/issues"
 
 [tool.poetry]
 name = "dsp-ifsc"
-version = "0.0.6"
+version = "0.0.7"
 description = "A small package with some utilities for DSP grade at IFSC - Campus Florianópolis"
 authors = [
     "João Mário Lago <joao.mcil2003@aluno.ifsc.edu.br>",
     "Alejo Perdomo Milar <alejo.pm@aluno.ifsc.edu.br>"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `dsp_ifsc-0.0.6/PKG-INFO` & `dsp_ifsc-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-ifsc
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small package with some utilities for DSP grade at IFSC - Campus Florianópolis
 Home-page: https://github.com/JoaoMario109/ifsc-dsp-2024
 License: MIT
 Author: João Mário Lago
 Author-email: joao.mcil2003@aluno.ifsc.edu.br
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

