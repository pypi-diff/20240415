# Comparing `tmp/surquest_split_balancer-0.0.1.tar.gz` & `tmp/surquest_split_balancer-0.0.2.tar.gz`

## Comparing `surquest_split_balancer-0.0.1.tar` & `surquest_split_balancer-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.1/package.base.dockerfile
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.1/surquest/utils/split_balancer/__init__.py
--rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.1/surquest/utils/split_balancer/errors.py
--rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.1/surquest/utils/split_balancer/split_balancer.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.1/test/pytest.ini
--rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.1/test/surquest/utils/split_balancer/test_split_balancer.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.1/LICENSE
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.1/README.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/package.base.dockerfile
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/surquest/utils/split_balancer/__init__.py
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/surquest/utils/split_balancer/errors.py
+-rw-r--r--   0        0        0     9232 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/surquest/utils/split_balancer/split_balancer.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/test/pytest.ini
+-rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/test/surquest/utils/split_balancer/test_split_balancer.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/README.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/PKG-INFO
```

### Comparing `surquest_split_balancer-0.0.1/package.base.dockerfile` & `surquest_split_balancer-0.0.2/package.base.dockerfile`

 * *Files identical despite different names*

### Comparing `surquest_split_balancer-0.0.1/.github/workflows/release.yml` & `surquest_split_balancer-0.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `surquest_split_balancer-0.0.1/.github/workflows/test.yml` & `surquest_split_balancer-0.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `surquest_split_balancer-0.0.1/surquest/utils/split_balancer/errors.py` & `surquest_split_balancer-0.0.2/surquest/utils/split_balancer/errors.py`

 * *Files identical despite different names*

### Comparing `surquest_split_balancer-0.0.1/surquest/utils/split_balancer/split_balancer.py` & `surquest_split_balancer-0.0.2/surquest/utils/split_balancer/split_balancer.py`

 * *Files 6% similar despite different names*

```diff
@@ -169,16 +169,14 @@
 
             avg["target"].append(
                 solver.Sum(x[val,self.groups[0]]*self.characteristics[ch][idx] for idx, val in enumerate(self.pool))/self.target_group_size
                 )
             avg["control"].append(
                 solver.Sum(x[val,self.groups[1]]*self.characteristics[ch][idx] for idx, val in enumerate(self.pool))/self.control_group_size
                 )
-            
-            print(":> ch", ch)
 
         # Define sum of avg characteristics for each group
         total_avg_target = solver.Sum(avg["target"][ch] for ch in range(n_characteristics))
         total_avg_control = solver.Sum(avg["control"][ch] for ch in range(n_characteristics))
 
         solver.Add(total_avg_target - total_avg_control <= dx)
         solver.Add(total_avg_control - total_avg_target <= dx)
@@ -216,30 +214,37 @@
 
             # Get vector of target and control variables
             vec_target = np.array([x[(i,self.groups[0])].solution_value() for i in self.pool])
             vec_control = np.array([x[(i,self.groups[1])].solution_value() for i in self.pool])
 
             # Get avg characteristics for each group
             avg = {
-                "target": [],
-                "control": []
+                "characteristics": [],
+                "total": None
+
             }
 
             n_characteristics = len(self.characteristics)
 
             for ch in range(n_characteristics):
 
                 vec_characteristics = np.array(self.characteristics[ch])
-                        
-                avg["target"].append(
-                    np.dot(vec_target, vec_characteristics)/self.target_group_size
-                    )
-                avg["control"].append(
-                     np.dot(vec_control, vec_characteristics)/self.control_group_size
-                    )
+
+                char_avg = {
+                    "target": np.dot(vec_target, vec_characteristics)/self.target_group_size,
+                    "control": np.dot(vec_control, vec_characteristics)/self.control_group_size
+                }
+
+                avg["characteristics"].append(char_avg)
+
+            # Get total avg characteristics
+            avg["total"] = {
+                "target": np.sum([avg["characteristics"][ch]["target"] for ch in range(n_characteristics)]),
+                "control": np.sum([avg["characteristics"][ch]["control"] for ch in range(n_characteristics)])
+            }
 
         else:
             logging.error("The problem does not have an optimal solution.")
             return None
         
         logging.info(f"Groups: {groups}")
         return {
```

### Comparing `surquest_split_balancer-0.0.1/test/surquest/utils/split_balancer/test_split_balancer.py` & `surquest_split_balancer-0.0.2/test/surquest/utils/split_balancer/test_split_balancer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 import random
+import time
 from surquest.utils.split_balancer import SplitBalancer
 from surquest.utils.split_balancer.errors import *
 
 
 target_group_size = 5
 control_group_size = 3
 in_target_group = [1, 2, 3]
@@ -111,8 +112,45 @@
 
             for unit in out_target_group:
                 assert unit not in groups["target"], f"Unit {unit} is in the target group: {groups['target']}"
 
             for unit in out_control_group:
                 assert unit not in groups["control"], f"Unit {unit} is in the control group: {groups['control']}"
 
-        
+    def test_benchmark(self):
+
+        n = 1000
+
+        for i in [10, 100, 500, 1000, 5000]:
+            for j in [1, 5, 10, 50]:
+
+                n = i
+                pool = range(n)
+                characteristics = []
+                for x in range(j):
+                    characteristics.append(
+                        [random.random() for _ in range(n)]
+                        )
+                        
+                target_group_size = 0.6*n
+                control_group_size = 0.2*n
+                in_target_group = None
+                in_control_group = None
+                out_target_group = None
+                out_control_group = None
+
+                split_balancer = SplitBalancer(
+                    pool=pool,
+                    characteristics=characteristics,
+                    target_group_size=target_group_size,
+                    control_group_size=control_group_size,
+                    in_target_group=in_target_group,
+                    in_control_group=in_control_group,
+                    out_target_group=out_target_group,
+                    out_control_group=out_control_group
+                )
+
+                start = time.process_time()
+                out = split_balancer.solve()
+                end = time.process_time()
+
+                print(f":> {i} - {j} - time {end-start}")
```

### Comparing `surquest_split_balancer-0.0.1/.gitignore` & `surquest_split_balancer-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `surquest_split_balancer-0.0.1/LICENSE` & `surquest_split_balancer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `surquest_split_balancer-0.0.1/README.md` & `surquest_split_balancer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `surquest_split_balancer-0.0.1/pyproject.toml` & `surquest_split_balancer-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "surquest-split-balancer"
-version = "0.0.1"
+version = "0.0.2"
 description = "A Python package for dividing a set of units into two most comparable groups based on their characteristics."
 authors = [
     {name= "Michal Švarc", email= "michal.svarc@surquest.com"}
 ]
 readme = "README.md"
 dependencies = [
     "ortools >= 9.9.3963",
```

### Comparing `surquest_split_balancer-0.0.1/PKG-INFO` & `surquest_split_balancer-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: surquest-split-balancer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for dividing a set of units into two most comparable groups based on their characteristics.
 Project-URL: Homepage, https://github.com/surquest/python-split-balancer
 Project-URL: Bug Tracker, https://github.com/surquest/python-split-balancer/issues
 Author-email: Michal Švarc <michal.svarc@surquest.com>
 License-File: LICENSE
 Requires-Dist: ortools>=9.9.3963
 Provides-Extra: test
```

