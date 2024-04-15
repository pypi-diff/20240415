# Comparing `tmp/surquest_split_balancer-0.0.2.tar.gz` & `tmp/surquest_split_balancer-0.0.3.tar.gz`

## Comparing `surquest_split_balancer-0.0.2.tar` & `surquest_split_balancer-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/package.base.dockerfile
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/surquest/utils/split_balancer/__init__.py
--rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/surquest/utils/split_balancer/errors.py
--rw-r--r--   0        0        0     9232 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/surquest/utils/split_balancer/split_balancer.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/test/pytest.ini
--rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/test/surquest/utils/split_balancer/test_split_balancer.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/LICENSE
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/README.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/package.base.dockerfile
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/app/main.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/app/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/app/schemas.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/surquest/utils/split_balancer/__init__.py
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/surquest/utils/split_balancer/errors.py
+-rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/surquest/utils/split_balancer/split_balancer.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/test/pytest.ini
+-rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/test/surquest/utils/split_balancer/test_split_balancer.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/README.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 surquest_split_balancer-0.0.3/PKG-INFO
```

### Comparing `surquest_split_balancer-0.0.2/package.base.dockerfile` & `surquest_split_balancer-0.0.3/package.base.dockerfile`

 * *Files identical despite different names*

### Comparing `surquest_split_balancer-0.0.2/.github/workflows/release.yml` & `surquest_split_balancer-0.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `surquest_split_balancer-0.0.2/.github/workflows/test.yml` & `surquest_split_balancer-0.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `surquest_split_balancer-0.0.2/surquest/utils/split_balancer/errors.py` & `surquest_split_balancer-0.0.3/surquest/utils/split_balancer/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,8 +52,16 @@
 class InvalidGroupSizeError(SplitBalancerError):
     """Exception raised when the group size is smaller than 1 or greater than the amount of units in the pool - 1."""
 
     def __init__(self, group_size, pool_size):
         self.group_size = group_size
         self.pool_size = pool_size
         message = f"Invalid group size: Group size ({self.group_size}) is smaller than 1 or greater than the amount of units in the pool ({self.pool_size}) - 1."
-        super().__init__(message)   
+        super().__init__(message)   
+
+
+class NoOptimalSolutionError(SplitBalancerError):
+    """Exception raised when there is no optimal solution to the split balancing problem."""
+
+    def __init__(self):
+
+        super().__init__("No optimal solution: There is no optimal solution to the split balancing problem.")
```

### Comparing `surquest_split_balancer-0.0.2/test/surquest/utils/split_balancer/test_split_balancer.py` & `surquest_split_balancer-0.0.3/test/surquest/utils/split_balancer/test_split_balancer.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 in_target_group = [1, 2, 3]
 in_control_group = [10]
 out_target_group = [9, 10]
 out_control_group = [4, 5]
 pool = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
 characteristics = {
     1: [
-        [0.4, 0.5, 0.6, 0.4, 0.6, 0.9, 0.1, 0.4, 0.6, 0.5]
+        [4, 5, 6, 4, 6, 9, 1, 4, 6, 5]
     ],
     2: [
-        [0.4, 0.5, 0.6, 0.4, 0.6, 0.9, 0.1, 0.4, 0.6, 0.5],
-        [0.2, 0.3, 0.4, 0.2, 0.4, 0.7, 0.1, 0.2, 0.4, 0.3]
+        [4, 5, 6, 4, 6, 9, 1, 4, 6, 5],
+        [2, 3, 4, 2, 4, 7, 1, 2, 4, 3]
     ]
 }
 
 big_N = 1000
 big_pool = range(big_N)
 characteristics["big"] = [
-    [random.random() for _ in range(big_N)],
-    [random.random() for _ in range(big_N)],
-    [random.random() for _ in range(big_N)]
+    [random.randrange(1, 100) for _ in range(big_N)],
+    [random.randrange(1, 100) for _ in range(big_N)],
+    [random.randrange(1, 100) for _ in range(big_N)]
 ]
-big_target_group_size = 0.8*big_N
-big_control_group_size = 0.1*big_N
+big_target_group_size = int(0.8*big_N)
+big_control_group_size = int(0.1*big_N)
 
 class TestSplitBalancer:
 
 
     @pytest.mark.parametrize(
         "target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics, expected",
         [
@@ -44,14 +44,15 @@
             (target_group_size, control_group_size, [1], [1], out_target_group, out_control_group, pool, characteristics.get(1), OverlappingUnitsError),
             (target_group_size, control_group_size, [1,2,3,4], [1,2,3,4], out_target_group, out_control_group, pool, characteristics.get(1), OverlappingUnitsError),
             (target_group_size, control_group_size, [1,2,3,4,5,6], [1,2,3,4,5,6], out_target_group, out_control_group, pool, characteristics.get(1), OverlappingUnitsError),
             (target_group_size, control_group_size, [1], in_control_group, [1], out_control_group, pool, characteristics.get(1), DuplicateUnitsError),
             (target_group_size, control_group_size, [1,2,3,4], in_control_group, [1,2,3,4], out_control_group, pool, characteristics.get(1), DuplicateUnitsError),
             (target_group_size, control_group_size, [1,2,3,4,5,6], in_control_group, [1,2,3,4,5,6], out_control_group, pool, characteristics.get(1), DuplicateUnitsError),
             (target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, in_control_group, pool, characteristics.get(1), DuplicateUnitsError),
+            (8, 2, in_target_group, [7, 8, 9, 10], out_target_group, out_control_group, pool, characteristics.get(1), NoOptimalSolutionError),
         ],
     )
     def test_failure(self, target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics, expected):
 
         try:
             split_balancer = SplitBalancer(
                 pool=pool,
@@ -60,26 +61,22 @@
                 control_group_size=control_group_size,
                 in_target_group=in_target_group,
                 in_control_group=in_control_group,
                 out_target_group=out_target_group,
                 out_control_group=out_control_group
             )
         except Exception as e:
-            assert isinstance(e, expected)
-            # assert str(e) == f"Insufficient units: pool size ({len(pool)}) is lower than the sum of target ({target_group_size}) + control ({control_group_size}) group sizes."
+            assert isinstance(e, expected), f"Expected {expected}, but got {type(e)}"
 
     @pytest.mark.parametrize(
         "target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics, expected",
         [
             (target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics.get(1), dict),
             (target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics.get(2), dict),
-            (8, 2, in_target_group, [7, 8, 9, 10], out_target_group, out_control_group, pool, characteristics.get(1), type(None)),
-            (big_target_group_size, big_control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, big_pool, characteristics.get("big"), dict),
-
-
+            (target_group_size, control_group_size, in_target_group, [7, 8, 9, 10], out_target_group, out_control_group, pool, characteristics.get(1), type(None)),
         ],
     )
     def test_success(self, target_group_size, control_group_size, in_target_group, in_control_group, out_target_group, out_control_group, pool, characteristics, expected):
         
         split_balancer = SplitBalancer(
             pool=pool,
             characteristics=characteristics,
@@ -87,15 +84,20 @@
             control_group_size=control_group_size,
             in_target_group=in_target_group,
             in_control_group=in_control_group,
             out_target_group=out_target_group,
             out_control_group=out_control_group
         )
 
-        results = split_balancer.solve()
+        results = None
+
+        try:
+            results = split_balancer.solve()
+        except NoOptimalSolutionError as e:
+            pass
 
         assert isinstance(results, expected)
 
         if expected is dict:
 
             groups = results.get("assignments")
 
@@ -114,29 +116,27 @@
                 assert unit not in groups["target"], f"Unit {unit} is in the target group: {groups['target']}"
 
             for unit in out_control_group:
                 assert unit not in groups["control"], f"Unit {unit} is in the control group: {groups['control']}"
 
     def test_benchmark(self):
 
-        n = 1000
-
-        for i in [10, 100, 500, 1000, 5000]:
-            for j in [1, 5, 10, 50]:
+        for i in [10, 100, 500, 1000, 1500, 2500, 5000]:
+            for j in [1, 2, 5, 10, 100]: # [1, 5, 10, 50]:
 
                 n = i
                 pool = range(n)
                 characteristics = []
                 for x in range(j):
                     characteristics.append(
-                        [random.random() for _ in range(n)]
+                        [random.randrange(0, 100) for _ in range(n)]
                         )
                         
-                target_group_size = 0.6*n
-                control_group_size = 0.2*n
+                target_group_size = int(0.6*n)
+                control_group_size = int(0.2*n)
                 in_target_group = None
                 in_control_group = None
                 out_target_group = None
                 out_control_group = None
 
                 split_balancer = SplitBalancer(
                     pool=pool,
@@ -145,12 +145,13 @@
                     control_group_size=control_group_size,
                     in_target_group=in_target_group,
                     in_control_group=in_control_group,
                     out_target_group=out_target_group,
                     out_control_group=out_control_group
                 )
 
-                start = time.process_time()
+                start = time.time()
                 out = split_balancer.solve()
-                end = time.process_time()
+                end = time.time()
 
-                print(f":> {i} - {j} - time {end-start}")
+                print(f":> {i} - {j} - time {end-start}")
+                print("-"*150)
```

### Comparing `surquest_split_balancer-0.0.2/.gitignore` & `surquest_split_balancer-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `surquest_split_balancer-0.0.2/LICENSE` & `surquest_split_balancer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `surquest_split_balancer-0.0.2/README.md` & `surquest_split_balancer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `surquest_split_balancer-0.0.2/pyproject.toml` & `surquest_split_balancer-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "surquest-split-balancer"
-version = "0.0.2"
+version = "0.0.3"
 description = "A Python package for dividing a set of units into two most comparable groups based on their characteristics."
 authors = [
     {name= "Michal Švarc", email= "michal.svarc@surquest.com"}
 ]
 readme = "README.md"
 dependencies = [
     "ortools >= 9.9.3963",
+    "requests"
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest>=8.1.1",
     "pytest-cov>=5.0.0"
 ]
```

### Comparing `surquest_split_balancer-0.0.2/PKG-INFO` & `surquest_split_balancer-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.3
 Name: surquest-split-balancer
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for dividing a set of units into two most comparable groups based on their characteristics.
 Project-URL: Homepage, https://github.com/surquest/python-split-balancer
 Project-URL: Bug Tracker, https://github.com/surquest/python-split-balancer/issues
 Author-email: Michal Švarc <michal.svarc@surquest.com>
 License-File: LICENSE
 Requires-Dist: ortools>=9.9.3963
+Requires-Dist: requests
 Provides-Extra: test
 Requires-Dist: pytest-cov>=5.0.0; extra == 'test'
 Requires-Dist: pytest>=8.1.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 ![GitHub](https://img.shields.io/github/license/surquest/python-split-balancer?style=flat-square)
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/surquest/python-split-balancer/test.yml?branch=main&style=flat-square)
```

