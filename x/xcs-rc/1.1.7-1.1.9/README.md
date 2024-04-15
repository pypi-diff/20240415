# Comparing `tmp/xcs-rc-1.1.7.tar.gz` & `tmp/xcs-rc-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcs-rc-1.1.7.tar", last modified: Thu Nov 23 08:12:19 2023, max compression
+gzip compressed data, was "xcs-rc-1.1.9.tar", last modified: Mon Apr 15 12:32:18 2024, max compression
```

## Comparing `xcs-rc-1.1.7.tar` & `xcs-rc-1.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-11-23 08:12:19.232672 xcs-rc-1.1.7/
--rw-rw-rw-   0        0        0    17893 2023-06-06 11:36:19.000000 xcs-rc-1.1.7/LICENSE
--rw-rw-rw-   0        0        0     4888 2023-11-23 08:12:19.231311 xcs-rc-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4295 2019-08-09 17:43:19.000000 xcs-rc-1.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-11-23 08:12:19.232672 xcs-rc-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      927 2023-11-23 08:12:01.000000 xcs-rc-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-23 08:12:19.220805 xcs-rc-1.1.7/xcs_rc/
--rw-rw-rw-   0        0        0    38597 2023-11-23 08:10:02.000000 xcs-rc-1.1.7/xcs_rc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-23 08:12:19.229763 xcs-rc-1.1.7/xcs_rc.egg-info/
--rw-rw-rw-   0        0        0     4888 2023-11-23 08:12:19.000000 xcs-rc-1.1.7/xcs_rc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-11-23 08:12:19.000000 xcs-rc-1.1.7/xcs_rc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-23 08:12:19.000000 xcs-rc-1.1.7/xcs_rc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-11-23 08:12:19.000000 xcs-rc-1.1.7/xcs_rc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-11-23 08:12:19.000000 xcs-rc-1.1.7/xcs_rc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 12:32:18.537255 xcs-rc-1.1.9/
+-rw-rw-rw-   0        0        0    17893 2023-06-06 11:36:19.000000 xcs-rc-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0     4888 2024-04-15 12:32:18.536195 xcs-rc-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4295 2019-08-09 17:43:19.000000 xcs-rc-1.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 12:32:18.537255 xcs-rc-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      927 2024-04-15 12:26:28.000000 xcs-rc-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:32:18.484722 xcs-rc-1.1.9/xcs_rc/
+-rw-rw-rw-   0        0        0    38815 2024-04-12 15:53:24.000000 xcs-rc-1.1.9/xcs_rc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:32:18.533929 xcs-rc-1.1.9/xcs_rc.egg-info/
+-rw-rw-rw-   0        0        0     4888 2024-04-15 12:32:18.000000 xcs-rc-1.1.9/xcs_rc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2024-04-15 12:32:18.000000 xcs-rc-1.1.9/xcs_rc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 12:32:18.000000 xcs-rc-1.1.9/xcs_rc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-15 12:32:18.000000 xcs-rc-1.1.9/xcs_rc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-15 12:32:18.000000 xcs-rc-1.1.9/xcs_rc.egg-info/top_level.txt
```

### Comparing `xcs-rc-1.1.7/LICENSE` & `xcs-rc-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xcs-rc-1.1.7/PKG-INFO` & `xcs-rc-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcs-rc
-Version: 1.1.7
+Version: 1.1.9
 Summary: Accuracy-based Learning Classifier Systems with Rule Combining
 Author: Nugroho Fredivianus
 Author-email: nuggfr@gmail.com
 License: Free for non-commercial use
 Keywords: machine learning,reinforcement learning,classifier systems,rule-based
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `xcs-rc-1.1.7/README.md` & `xcs-rc-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `xcs-rc-1.1.7/setup.py` & `xcs-rc-1.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='xcs-rc',
-    version='1.1.7',
+    version='1.1.9',
     license='Free for non-commercial use',
     author='Nugroho Fredivianus',
     author_email='nuggfr@gmail.com',
     description='Accuracy-based Learning Classifier Systems with Rule Combining',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(include=['xcs_rc']),
```

### Comparing `xcs-rc-1.1.7/xcs_rc/__init__.py` & `xcs-rc-1.1.9/xcs_rc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,14 +519,18 @@
     def combine_act(self, act):
         minexp = self.owner.minexp
         predtol = self.owner.predtol
         beta = self.owner.beta
 
         cset = ClassifierSet(name=f"[C:{act}]")
         cset.cl = [cl for cl in self.cl if cl.act == act]
+
+        if len(cset.cl) < 2:
+            return
+
         pressing = True
         while pressing:
             pressing = False
             cset.sort()
             parent1 = [cl for cl in cset.cl if cl.exp >= minexp]
             for p1 in parent1:
                 parent2 = [cl for cl in parent1 if cl != p1 and abs(p1.pred - cl.pred) <= predtol]
@@ -585,17 +589,19 @@
 
     def get_header(self):
         head = f"id{SEPARATOR}cond{SEPARATOR}"
         if not self.owner.binaries:
             for i in range(len(self.cl[0].cond) - 1):
                 head += SEPARATOR
         head += SEPARATOR.join(["act", "pred", "fit", "prederr", "num", "exp", "actsetsize"])
-
         return head
 
+    def to_list(self):
+        return [cl.to_list() for cl in self.cl]
+
     def print(self, title="", header=True, per_action=False):
         if per_action:
             counts = []
             for i in range(self.owner.num_actions):
                 counts.append(sum(cl.act == i for cl in self.cl))
             print(counts, " - Sum:", sum(counts))
             return
@@ -831,14 +837,18 @@
         beta = self.owner.beta
         exp_lim = 1 / beta
         if self.exp <= int(exp_lim):
             self.prederr = abs(self.pred - pred_init) / self.exp
         else:
             self.prederr = (abs(self.pred - pred_init) / exp_lim) * pow(1 - beta, self.exp - int(exp_lim))
 
+    def to_list(self):
+        return [[[c[0], c[-1]] for c in self.cond], self.act, self.pred,
+                self.fit, self.prederr, self.num, self.exp, self.actsetsize]
+
     def printable_cond(self):
         str_cond = ""
         if self.owner.binaries:
             str_cond = '"'
             for sc in self.cond:
                 str_cond += "#" if sc[0] != sc[1] else "0" if sc[0] == 0.0 else "1"
             str_cond += '"'
@@ -1019,33 +1029,27 @@
     for v in val:
         c = 0.000 if v == '0' else 1.000
         cond.append(c)
     return cond
 
 
 def floatify(state):
-    my_separator = ""
-    number = (int, int64, float, float64, complex)
+    my_range_separator = ""
     cond = []
     if isinstance(state, str):
         if state[0] == '[':
             states = state.split('],[')
             for s in states:
                 s = s.replace('[', '').replace(']', '')
-                a = [0, 0]
-                if len(my_separator) == 0 and not s.replace(".", "", 1).isdigit():
+                if len(my_range_separator) == 0 and not s.replace(".", "", 1).isdigit():
                     check = re.findall("[^0-9.-]+", s)
                     if len(check) > 0:
-                        my_separator = check[0]
+                        my_range_separator = check[0]
 
-                if s.count(my_separator) == 1:
-                    a = s.split(my_separator)
-                else:
-                    a[0] = s
-                    a[1] = s
+                a = s.split(my_range_separator) if s.count(my_range_separator) == 1 else [s, s]
                 cond.append([float(a[0]), float(a[1])])
         else:
             if len(re.findall("[^01#]", state)) > 0:
                 print("Cl cond: not a binary string.")
                 return False
 
             for s in state.replace('"', ''):
@@ -1053,14 +1057,15 @@
                     cond.append([0.00, 0.00])
                 elif s == "1":
                     cond.append([1.00, 1.00])
                 else:
                     cond.append([0.00, 1.00])
 
     elif isinstance(state, list):
+        number = (int, int64, float, float64, complex)
         for s in state:
             if isinstance(s, number):
                 s = int(s) if isinstance(s, int64) else float(s) if isinstance(s, float64) else s
                 cond.append([s, s])
             elif isinstance(s, list):
                 cond.append(s)
```

### Comparing `xcs-rc-1.1.7/xcs_rc.egg-info/PKG-INFO` & `xcs-rc-1.1.9/xcs_rc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcs-rc
-Version: 1.1.7
+Version: 1.1.9
 Summary: Accuracy-based Learning Classifier Systems with Rule Combining
 Author: Nugroho Fredivianus
 Author-email: nuggfr@gmail.com
 License: Free for non-commercial use
 Keywords: machine learning,reinforcement learning,classifier systems,rule-based
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

