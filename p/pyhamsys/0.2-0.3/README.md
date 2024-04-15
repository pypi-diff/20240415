# Comparing `tmp/pyhamsys-0.2.tar.gz` & `tmp/pyhamsys-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhamsys-0.2.tar", last modified: Fri Oct 20 15:21:11 2023, max compression
+gzip compressed data, was "pyhamsys-0.3.tar", last modified: Mon Apr 15 09:30:24 2024, max compression
```

## Comparing `pyhamsys-0.2.tar` & `pyhamsys-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-10-20 15:21:11.559578 pyhamsys-0.2/
--rw-r--r--   0 cchandre   (501) staff       (20)     1304 2023-04-05 14:49:59.000000 pyhamsys-0.2/LICENSE
--rw-r--r--   0 cchandre   (501) staff       (20)    12226 2023-10-20 15:21:11.559277 pyhamsys-0.2/PKG-INFO
--rw-r--r--   0 cchandre   (501) staff       (20)    11413 2023-10-20 15:20:51.000000 pyhamsys-0.2/README.md
-drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-10-20 15:21:11.556093 pyhamsys-0.2/pyhamsys/
-drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-10-20 15:21:11.557467 pyhamsys-0.2/pyhamsys/src/
-drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2023-10-20 15:21:11.558854 pyhamsys-0.2/pyhamsys/src/pyhamsys.egg-info/
--rw-r--r--   0 cchandre   (501) staff       (20)    12226 2023-10-20 15:21:11.000000 pyhamsys-0.2/pyhamsys/src/pyhamsys.egg-info/PKG-INFO
--rw-r--r--   0 cchandre   (501) staff       (20)      275 2023-10-20 15:21:11.000000 pyhamsys-0.2/pyhamsys/src/pyhamsys.egg-info/SOURCES.txt
--rw-r--r--   0 cchandre   (501) staff       (20)        1 2023-10-20 15:21:11.000000 pyhamsys-0.2/pyhamsys/src/pyhamsys.egg-info/dependency_links.txt
--rw-r--r--   0 cchandre   (501) staff       (20)       12 2023-10-20 15:21:11.000000 pyhamsys-0.2/pyhamsys/src/pyhamsys.egg-info/requires.txt
--rw-r--r--   0 cchandre   (501) staff       (20)        9 2023-10-20 15:21:11.000000 pyhamsys-0.2/pyhamsys/src/pyhamsys.egg-info/top_level.txt
--rw-r--r--   0 cchandre   (501) staff       (20)    20759 2023-10-20 14:58:01.000000 pyhamsys-0.2/pyhamsys/src/pyhamsys.py
--rw-r--r--   0 cchandre   (501) staff       (20)       38 2023-10-20 15:21:11.559672 pyhamsys-0.2/setup.cfg
--rw-r--r--   0 cchandre   (501) staff       (20)     1127 2023-10-20 15:19:26.000000 pyhamsys-0.2/setup.py
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2024-04-15 09:30:24.474318 pyhamsys-0.3/
+-rw-r--r--   0 cchandre   (501) staff       (20)     1304 2023-04-05 14:49:59.000000 pyhamsys-0.3/LICENSE
+-rw-r--r--   0 cchandre   (501) staff       (20)    12226 2024-04-15 09:30:24.473925 pyhamsys-0.3/PKG-INFO
+-rw-r--r--   0 cchandre   (501) staff       (20)    11413 2023-10-20 15:20:51.000000 pyhamsys-0.3/README.md
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2024-04-15 09:30:24.470272 pyhamsys-0.3/pyhamsys/
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2024-04-15 09:30:24.471831 pyhamsys-0.3/pyhamsys/src/
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2024-04-15 09:30:24.473439 pyhamsys-0.3/pyhamsys/src/pyhamsys.egg-info/
+-rw-r--r--   0 cchandre   (501) staff       (20)    12226 2024-04-15 09:30:24.000000 pyhamsys-0.3/pyhamsys/src/pyhamsys.egg-info/PKG-INFO
+-rw-r--r--   0 cchandre   (501) staff       (20)      275 2024-04-15 09:30:24.000000 pyhamsys-0.3/pyhamsys/src/pyhamsys.egg-info/SOURCES.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)        1 2024-04-15 09:30:24.000000 pyhamsys-0.3/pyhamsys/src/pyhamsys.egg-info/dependency_links.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)       12 2024-04-15 09:30:24.000000 pyhamsys-0.3/pyhamsys/src/pyhamsys.egg-info/requires.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)        9 2024-04-15 09:30:24.000000 pyhamsys-0.3/pyhamsys/src/pyhamsys.egg-info/top_level.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)    22136 2023-10-24 14:15:51.000000 pyhamsys-0.3/pyhamsys/src/pyhamsys.py
+-rw-r--r--   0 cchandre   (501) staff       (20)       38 2024-04-15 09:30:24.474421 pyhamsys-0.3/setup.cfg
+-rw-r--r--   0 cchandre   (501) staff       (20)     1127 2024-04-15 09:29:02.000000 pyhamsys-0.3/setup.py
```

### Comparing `pyhamsys-0.2/LICENSE` & `pyhamsys-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhamsys-0.2/PKG-INFO` & `pyhamsys-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhamsys
-Version: 0.2
+Version: 0.3
 Summary: Some tools for Hamiltonian systems
 Home-page: http://github.com/cchandre/pyhamsys
 Author: Cristel Chandre
 Author-email: cristel.chandre@cnrs.fr
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Education
```

### Comparing `pyhamsys-0.2/README.md` & `pyhamsys-0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyhamsys-0.2/pyhamsys/src/pyhamsys.egg-info/PKG-INFO` & `pyhamsys-0.3/pyhamsys/src/pyhamsys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhamsys
-Version: 0.2
+Version: 0.3
 Summary: Some tools for Hamiltonian systems
 Home-page: http://github.com/cchandre/pyhamsys
 Author: Cristel Chandre
 Author-email: cristel.chandre@cnrs.fr
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Education
```

### Comparing `pyhamsys-0.2/pyhamsys/src/pyhamsys.py` & `pyhamsys-0.3/pyhamsys/src/pyhamsys.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import numpy as xp
+import matplotlib.pyplot as plt
+from scipy.optimize import curve_fit
+from scipy.stats import linregress
+from sklearn.metrics import r2_score
 from scipy.fft import rfft, irfft, rfftfreq
 from typing import Callable, Union, Tuple
 from scipy.optimize import OptimizeResult
 import sympy as sp
 from functools import partial 
 
 class OdeSolution(OptimizeResult):
@@ -50,15 +54,25 @@
 		if not by_var:
 			return [y[:np], y[np:2*np], y[2*np:]]
 		return [y[:np//2], y[np//2:np], y[np:3*np//2], y[3*np//2:2*np], y[2*np:]]
 	
 	def _create_function(self, t:float, y:xp.ndarray, eqn:Callable) -> xp.ndarray:
 		y_ = xp.split(y, 2)
 		return xp.asarray(eqn(y_[0], y_[1], t)).flatten()
-
+	
+	def rectify_sol(self, sol:OdeSolution, check_energy:bool=False) -> OdeSolution:
+		if not check_energy:
+			return sol
+		if self._time_dependent:
+			vec = self._split(sol.y, ext=False, check_energy=True)
+			sol.y = xp.concatenate((vec[0], vec[1]), axis=0)
+			sol.k = vec[2]
+		sol.err = self.compute_energy(sol)
+		return sol
+	
 	def compute_vector_field(self, hamiltonian:Callable, output:bool=False) -> None:
 		q = sp.symbols('q0:%d'%self._ndof) if self._ndof>=2 else sp.Symbol('q')
 		p = sp.symbols('p0:%d'%self._ndof) if self._ndof>=2 else sp.Symbol('p')
 		t = sp.Symbol('t')
 		energy = sp.lambdify([q, p, t], hamiltonian(q, p, t))
 		self.hamiltonian = partial(self._create_function, eqn=energy)
 		eqn = sp.simplify(sp.derive_by_array(hamiltonian(q, p, t), [q, p]).doit())
@@ -78,14 +92,38 @@
 			raise ValueError("In order to check energy, the attribute 'hamiltonian' must be provided.")
 		val_h = self.hamiltonian(sol.t[xp.newaxis], sol.y)
 		if self._time_dependent:
 			val_h += sol.k
 			val_h -= val_h[:, 0][:, xp.newaxis]
 		return xp.max(xp.abs(val_h - val_h[:, 0][:, xp.newaxis])) if maxerror else val_h 
 
+def compute_msd(sol:OdeSolution, plot_data:bool=False, output_r2:bool=False):
+	x, y = xp.split(sol.y, 2)
+	nt = len(sol.t)
+	r2 = xp.zeros(nt)
+	for _ in range(nt):
+		r2[_] = ((x[:, _:] - x[:, :-_ if _ else None])**2 + (y[:, _:] - y[:, :-_ if _ else None])**2).mean()
+	t_win, r2_win = sol.t[nt//8:7*nt//8], r2[nt//8:7*nt//8]
+	res = linregress(t_win, r2_win)
+	diff_data = [res.slope, res.intercept, res.rvalue**2]
+	func_fit = lambda t, a, b: (a * t)**b
+	popt = curve_fit(func_fit, t_win, r2_win, bounds=((0, 0.25), (xp.inf, 3)))[0]
+	r2_fit = func_fit(t_win, *popt)
+	interp_data = [*popt, r2_score(r2_win, r2_fit)]
+	if plot_data:
+		plt.plot(sol.t, r2, ':', color='r', lw=1)
+		plt.plot(t_win, r2_win, '-', color='r', lw=2)
+		plt.plot(t_win, r2_fit, '-.', color='r', lw=2)
+		plt.xlabel('$t$')
+		plt.ylabel('$r^2$')
+		plt.show()
+	if output_r2:
+		return sol.t, r2, diff_data, interp_data
+	return diff_data, interp_data
+
 def antiderivative(vec:xp.ndarray, N:int=2**10) -> xp.ndarray:
 	nu = rfftfreq(N, d=1/N)
 	div = xp.divide(1, 1j * nu, where=nu!=0)
 	div[0] = 0
 	return irfft(rfft(vec, axis=-1) * div, axis=-1)
 
 def padwrap(vec:xp.ndarray) -> xp.ndarray:
@@ -466,15 +504,15 @@
 		if check_energy_:
 			y_[-1] += h * hs.k_dot(t, y_[0])
 		return xp.concatenate([_ for _ in y_], axis=None)
 	
 	if not hasattr(hs, 'y_dot'):
 		raise ValueError("The attribute 'y_dot' must be provided.")
 	if check_energy_ and not hasattr(hs, 'k_dot'):
-		raise ValueError("In order to check energy for a time-dependent system, the attrribute 'k_dot' must be provided.")
+		raise ValueError("In order to check energy for a time-dependent system, the attribute 'k_dot' must be provided.")
 	y_ = xp.tile(y0, 2)
 	if check_energy_:
 		y_ = xp.concatenate((y_, xp.zeros(len(y0)//(2*hs._ndof) )), axis=None)
 	sol = solve_ivp_symp(_chi_ext, _chi_ext_star, t_span, y_, method=method, step=step, t_eval=t_eval, command=command)
 	y_ = hs._split(sol.y, by_var=True, check_energy=check_energy_)
 	sol.y = xp.concatenate(((y_[0] + y_[2]) / 2, (y_[1] + y_[3]) / 2), axis=0)
 	if check_energy_:
```

### Comparing `pyhamsys-0.2/setup.py` & `pyhamsys-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhamsys',
-    version='0.2',
+    version='0.3',
     description='Some tools for Hamiltonian systems',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url='http://github.com/cchandre/pyhamsys',
     classifiers=[
       'Programming Language :: Python :: 3',
```

