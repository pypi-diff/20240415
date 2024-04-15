# Comparing `tmp/dsp_ifsc-0.0.8.tar.gz` & `tmp/dsp_ifsc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_ifsc-0.0.8.tar", max compression
+gzip compressed data, was "dsp_ifsc-0.0.9.tar", max compression
```

## Comparing `dsp_ifsc-0.0.8.tar` & `dsp_ifsc-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.8/LICENSE
--rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.8/README.md
--rw-r--r--   0        0        0        0 2024-04-14 21:18:08.641250 dsp_ifsc-0.0.8/dsp_ifsc/__init__.py
--rw-r--r--   0        0        0     2281 2024-04-14 23:28:11.770848 dsp_ifsc-0.0.8/dsp_ifsc/sequence.py
--rw-r--r--   0        0        0    12337 2024-04-14 23:28:33.847900 dsp_ifsc-0.0.8/dsp_ifsc/signal.py
--rw-r--r--   0        0        0     1007 2024-04-14 23:31:34.274392 dsp_ifsc-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.9/LICENSE
+-rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 21:18:08.641250 dsp_ifsc-0.0.9/dsp_ifsc/__init__.py
+-rw-r--r--   0        0        0     3581 2024-04-14 23:40:08.016794 dsp_ifsc-0.0.9/dsp_ifsc/sequence.py
+-rw-r--r--   0        0        0    14765 2024-04-15 06:39:14.304910 dsp_ifsc-0.0.9/dsp_ifsc/signal.py
+-rw-r--r--   0        0        0     1558 2024-04-15 05:48:01.248926 dsp_ifsc-0.0.9/dsp_ifsc/system.py
+-rw-r--r--   0        0        0     1007 2024-04-15 06:41:27.597459 dsp_ifsc-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.9/PKG-INFO
```

### Comparing `dsp_ifsc-0.0.8/LICENSE` & `dsp_ifsc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_ifsc-0.0.8/dsp_ifsc/signal.py` & `dsp_ifsc-0.0.9/dsp_ifsc/signal.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,16 +27,17 @@
 
         if len(n) < len(x):
             raise ValueError("The n sequence must have the same length or more than x sequence")
 
         if len(n) > len(x):
             x = numpy.pad(x, (0, len(n) - len(x)))
 
-        self.x = x
-        self.n = n
+        self.x = numpy.array(x)
+        self.n = numpy.array(n)
+
 
     # Methods
 
     def _adjust_signals(self, other: Self) -> numpy.ndarray:
         """
         Adjusts the n sequence of two signals.
         Args:
@@ -44,21 +45,46 @@
 
         Returns:
             n: The adjusted n sequence.
         """
 
         n = numpy.arange(min(self.n.min(0), other.n.min(0)), max(self.n.max(0), other.n.max(0)) + 1)
         y1 = numpy.zeros(len(n))
-        y1[numpy.logical_and((n >= self.n.min(0)), (n <= self.n.max(0)))] = self.x
+        y1[numpy.logical_and((n >= self.n.min(0)), (n <= self.n.max(0)))] = self.x.copy()
         y2 = numpy.zeros(len(n))
-        y2[numpy.logical_and((n >= other.n.min(0)), (n <= other.n.max(0)))] = other.x
+        y2[numpy.logical_and((n >= other.n.min(0)), (n <= other.n.max(0)))] = other.x.copy()
 
         return n, y1, y2
 
 
+    def tile(self, k: int) -> 'Signal':
+        """
+        Tiles the signal.
+        Args:
+            n: The sequence of n values.
+            k: The number of tiles.
+
+        Returns:
+            signal: The tiled Signal class.
+        """
+
+        # Check if n is equally spaced
+        if len(self.n) < 2:
+            raise ValueError('n must have at least two elements')
+
+        diff = self.n[1] - self.n[0]
+        if not numpy.all(numpy.diff(self.n) == diff):
+            raise ValueError('n must be equally spaced')
+
+        y = numpy.tile(self.x, k)
+        _n = [ self.n[0] + i * diff for i in range(len(y)) ]
+
+        return Signal(y, _n)
+
+
     def add(self, other: Self) -> 'Signal':
         """
         Implements y(n) = x1(n) + x2(n)
         Args:
             signal: The Signal class to be added.
 
         Returns:
@@ -115,25 +141,25 @@
 
         n, y1, y2 = self._adjust_signals(other)
         y = y1 / y2
 
         return Signal(y, n)
 
 
-    def shift(self, k: int) -> 'Signal':
+    def shift(self, k: int | float) -> 'Signal':
         """
         Implements y(n) = x(n - k)
         Args:
             k: The shift value.
 
         Returns:
             signal: The shifted Signal class.
         """
 
-        y = self.x
+        y = self.x.copy()
         n = self.n + k
 
         return Signal(y, n)
 
 
     def fold(self) -> 'Signal':
         """
@@ -152,31 +178,47 @@
         """
         Implements y(n) = -x(n)
         Returns:
             signal: The negated Signal class.
         """
 
         y = -self.x
-        n = self.n
+        n = self.n.copy()
 
         return Signal(y, n)
 
 
+    def scale(self, k: int) -> 'Signal':
+        """
+        Implements y(n) = x(k * n)
+        Args:
+            k: The scale factor.
+
+        Returns:
+            signal: The scaled Signal class.
+        """
+
+        # Subsample the signal values with a step of k
+        y = self.x[::k]
+
+        return Signal(y, self.n)
+
+
     def convolution(self, other: Self) -> 'Signal':
         """
         Implements y(n) = x(n) * h(n)
         Args:
             signal: The Signal class to be convolved.
 
         Returns:
             signal: The convolved Signal class.
         """
 
         y = numpy.convolve(self.x, other.x)
-        n = numpy.arange(self.n.min(0) + other.n.min(0), self.n.max(0) + other.n.max(0) + 1)
+        n = numpy.arange(self.n.min() + other.n.min(), self.n.max() + other.n.max() + 1)
 
         return Signal(y, n)
 
 
     def correlation(self, other: Self) -> 'Signal':
         """
         Implements y(n) = x(n) * h(-n)
@@ -184,20 +226,20 @@
             signal: The Signal class to be correlated.
 
         Returns:
             signal: The correlated Signal class.
         """
 
         y = numpy.correlate(self.x, other.x)
-        n = numpy.arange(self.n.min(0) - other.n.max(0), self.n.max(0) - other.n.min(0) + 1)
+        n = numpy.arange(self.n.min() + other.n.min(), self.n.max() + other.n.max() + 1)
 
         return Signal(y, n)
 
 
-    def stem(self, plot: Optional[Axes] = None, auto_plot: Optional[bool] = True) -> Axes:
+    def stem(self, title: Optional[str] = r'Signal', plot: Optional[Axes] = None, auto_plot: Optional[bool] = True) -> Axes:
         """
         Plots the signal.
         """
 
         if plot is None:
             plot = plt.subplot()
 
@@ -207,15 +249,15 @@
         plot.yaxis.set_major_locator(MaxNLocator(nbins = 'auto'))  # Automatically adjust y-ticks
         plot.xaxis.set_minor_locator(AutoMinorLocator())
         plot.yaxis.set_minor_locator(AutoMinorLocator())
         plot.grid(True, which = 'both', linestyle = '--', linewidth = 0.5, alpha = 0.7)
         # Details
         plot.set_xlabel('n')
         plot.set_ylabel('x(n)')
-        plot.set_title('Signal')
+        plot.set_title(title)
 
         if auto_plot:
             plt.show()
 
         return plot
 
 
@@ -310,38 +352,38 @@
         Returns:
             signal: The negative Signal class.
         """
 
         return self.negate()
 
 
-    def __lshift__(self, k: int) -> 'Signal':
+    def __lshift__(self, k: int | float) -> 'Signal':
         """
         Overloads the << operator.
         Args:
             k: The shift value.
 
         Returns:
             signal: The shifted Signal class.
         """
 
-        return self.shift(k)
+        return self.shift(-k)
 
 
-    def __rshift__(self, k: int) -> 'Signal':
+    def __rshift__(self, k: int | float) -> 'Signal':
         """
         Overloads the >> operator.
         Args:
             k: The shift value.
 
         Returns:
             signal: The shifted Signal class.
         """
 
-        return self.shift(-k)
+        return self.shift(k)
 
 
     def __invert__(self) -> 'Signal':
         """
         Overloads the ~ operator.
         Returns:
             signal: The folded Signal class.
@@ -444,14 +486,28 @@
         Returns:
             signal: The Signal class.
         """
 
         return other.correlation(self)
 
 
+    def __getitem__(self, key):
+        """
+        Overloads the [] operator.
+
+        Returns:
+            signal: The Signal class.
+        """
+
+        if isinstance(key, slice):
+            return Signal(self.x[key], self.n[key])
+
+        return self.x[key]
+
+
     # Static methods
 
     @staticmethod
     def from_zeros(n: numpy.ndarray) -> 'Signal':
         """
         Generates a zero signal.
         Args:
@@ -497,43 +553,84 @@
 
         x, _n = sequence.impulse(position, n.min(), n.max())
 
         return Signal(x, _n)
 
 
     @staticmethod
-    def from_step(n: numpy.ndarray, position: int = 0):
+    def from_step(n: numpy.ndarray, position: int = 0) -> 'Signal':
         """
         Generates a step signal.
         Returns:
             signal: The step Signal class.
         """
 
         x, _n = sequence.step(position, n.min(), n.max())
 
         return Signal(x, _n)
 
 
     @staticmethod
-    def from_ramp(slope: float, n: numpy.ndarray, position: int = 0):
+    def from_ramp(slope: float, n: numpy.ndarray, position: int = 0) -> 'Signal':
         """
         Generates a ramp signal.
         Returns:
             signal: The ramp Signal class.
         """
 
         x, _n = sequence.ramp(slope, position, n.min(), n.max())
 
         return Signal(x, _n)
 
 
     @staticmethod
-    def from_exponential(amplitude: float, alpha: float, n: numpy.ndarray, position: int = 0):
+    def from_exponential(alpha: float, n: numpy.ndarray, position: int = 0, amplitude: float = 1.0) -> 'Signal':
         """
         Generates an exponential signal.
         Returns:
             signal: The exponential Signal class.
         """
 
         x, _n = sequence.exponential(amplitude, alpha, position, n.min(), n.max())
 
         return Signal(x, _n)
+
+
+    @staticmethod
+    def from_sine(omega: float, n: numpy.ndarray, phase: float = 0.0, amplitude: float = 1.0) -> 'Signal':
+        """
+        Generates a sine signal.
+        Returns:
+            signal: The sine Signal class.
+        """
+
+        x, _n = sequence.sine(amplitude, omega, phase, n.min(), n.max())
+
+        return Signal(x, _n)
+
+
+    @staticmethod
+    def from_cosine(omega: float, n: numpy.ndarray, phase: float = 0.0, amplitude: float = 1.0) -> 'Signal':
+        """
+        Generates a cosine signal.
+        Returns:
+            signal: The cosine Signal class.
+        """
+
+        x, _n = sequence.cosine(amplitude, omega, phase, n.min(), n.max())
+
+        return Signal(x, _n)
+
+
+    @staticmethod
+    def from_tile(x: numpy.ndarray, n: numpy.ndarray, k: int) -> 'Signal':
+        """
+        Tiles the signal.
+        Args:
+            n: The sequence of n values.
+            k: The number of tiles.
+
+        Returns:
+            signal: The tiled Signal class.
+        """
+
+        return Signal(x, n).tile(k)
```

### Comparing `dsp_ifsc-0.0.8/pyproject.toml` & `dsp_ifsc-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project.urls]
 Homepage = "https://github.com/JoaoMario109/ifsc-dsp-2024"
 Issues = "https://github.com/JoaoMario109/ifsc-dsp-2024/issues"
 
 [tool.poetry]
 name = "dsp-ifsc"
-version = "0.0.8"
+version = "0.0.9"
 description = "A small package with some utilities for DSP grade at IFSC - Campus Florianópolis"
 authors = [
     "João Mário Lago <joao.mcil2003@aluno.ifsc.edu.br>",
     "Alejo Perdomo Milar <alejo.pm@aluno.ifsc.edu.br>"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `dsp_ifsc-0.0.8/PKG-INFO` & `dsp_ifsc-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-ifsc
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small package with some utilities for DSP grade at IFSC - Campus Florianópolis
 Home-page: https://github.com/JoaoMario109/ifsc-dsp-2024
 License: MIT
 Author: João Mário Lago
 Author-email: joao.mcil2003@aluno.ifsc.edu.br
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

