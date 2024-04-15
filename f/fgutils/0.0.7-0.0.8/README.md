# Comparing `tmp/fgutils-0.0.7.tar.gz` & `tmp/fgutils-0.0.8.tar.gz`

## Comparing `fgutils-0.0.7.tar` & `fgutils-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 fgutils-0.0.7/.coveragerc
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 fgutils-0.0.7/lint.sh
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 fgutils-0.0.7/requirements.txt
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 fgutils-0.0.7/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 fgutils-0.0.7/.github/workflows/test-and-lint.yml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 fgutils-0.0.7/fgutils/__init__.py
--rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 fgutils-0.0.7/fgutils/fgconfig.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 fgutils-0.0.7/fgutils/mapping.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fgutils-0.0.7/fgutils/parse.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 fgutils-0.0.7/fgutils/permutation.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 fgutils-0.0.7/fgutils/query.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fgutils-0.0.7/fgutils/rdkit.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 fgutils-0.0.7/fgutils/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fgutils-0.0.7/test/__init__.py
--rw-r--r--   0        0        0     9422 2020-02-02 00:00:00.000000 fgutils-0.0.7/test/test_fgconfig.py
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 fgutils-0.0.7/test/test_mapping.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 fgutils-0.0.7/test/test_parse.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 fgutils-0.0.7/test/test_permutation.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 fgutils-0.0.7/test/test_query.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 fgutils-0.0.7/test/test_utils.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 fgutils-0.0.7/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fgutils-0.0.7/LICENSE
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 fgutils-0.0.7/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 fgutils-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 fgutils-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 fgutils-0.0.8/.coveragerc
+-rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 fgutils-0.0.8/lint.sh
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 fgutils-0.0.8/requirements.txt
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 fgutils-0.0.8/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 fgutils-0.0.8/.github/workflows/test-and-lint.yml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/__init__.py
+-rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/fgconfig.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/mapping.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/parse.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/permutation.py
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/query.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/rdkit.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fgutils-0.0.8/test/__init__.py
+-rw-r--r--   0        0        0     9422 2020-02-02 00:00:00.000000 fgutils-0.0.8/test/test_fgconfig.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 fgutils-0.0.8/test/test_mapping.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 fgutils-0.0.8/test/test_parse.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 fgutils-0.0.8/test/test_permutation.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 fgutils-0.0.8/test/test_query.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 fgutils-0.0.8/test/test_utils.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 fgutils-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fgutils-0.0.8/LICENSE
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 fgutils-0.0.8/README.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 fgutils-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 fgutils-0.0.8/PKG-INFO
```

### Comparing `fgutils-0.0.7/.github/workflows/publish-package.yml` & `fgutils-0.0.8/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/.github/workflows/test-and-lint.yml` & `fgutils-0.0.8/.github/workflows/test-and-lint.yml`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/fgutils/fgconfig.py` & `fgutils-0.0.8/fgutils/fgconfig.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/fgutils/mapping.py` & `fgutils-0.0.8/fgutils/mapping.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/fgutils/parse.py` & `fgutils-0.0.8/fgutils/parse.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/fgutils/permutation.py` & `fgutils-0.0.8/fgutils/permutation.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/fgutils/query.py` & `fgutils-0.0.8/fgutils/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,23 +95,14 @@
                 assert atom_id in indices
                 for i in indices:
                     if i in fg_candidate_ids:
                         fg_candidate_ids.remove(i)
                     elif i in unidentified_ids:
                         unidentified_ids.remove(i)
                 groups.append((node.fgconfig.name, indices))
-        if len(unidentified_ids) > 0:
-            raise RuntimeError(
-                "Could not find a functional group for atom(s) {}.".format(
-                    [
-                        "{}@{}".format(graph.nodes[i]["symbol"], i)
-                        for i in unidentified_ids
-                    ]
-                )
-            )
         return groups
 
     def get(self, value) -> list[tuple[str, list[int]]]:
         mol_graph = None
         if isinstance(value, nx.Graph):
             mol_graph = value
         elif self.use_smiles:
```

### Comparing `fgutils-0.0.7/fgutils/rdkit.py` & `fgutils-0.0.8/fgutils/rdkit.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/fgutils/utils.py` & `fgutils-0.0.8/fgutils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,13 +38,13 @@
         if n_sym not in ["R", "H"]
     ]
     for n_id, n_sym in nodes:
         assert (
             n_sym in valence_table.keys()
         ), "Element {} not found in valence table.".format(n_sym)
         bond_cnt = sum([b for _, _, b in graph.edges(n_id, data="bond")])  # type: ignore
+        # h_cnt can be negative; aromaticity is complicated, we just ignore that
         h_cnt = int(8 - valence_table[n_sym] - bond_cnt)
-        assert h_cnt >= 0, "Negative hydrogen count."
         for h_id in range(len(graph), len(graph) + h_cnt):
             graph.add_node(h_id, symbol="H")
             graph.add_edge(n_id, h_id, bond=1)
     return graph
```

### Comparing `fgutils-0.0.7/test/test_fgconfig.py` & `fgutils-0.0.8/test/test_fgconfig.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/test/test_mapping.py` & `fgutils-0.0.8/test/test_mapping.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/test/test_parse.py` & `fgutils-0.0.8/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/test/test_permutation.py` & `fgutils-0.0.8/test/test_permutation.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/test/test_query.py` & `fgutils-0.0.8/test/test_query.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/.gitignore` & `fgutils-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/LICENSE` & `fgutils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/README.md` & `fgutils-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.7/pyproject.toml` & `fgutils-0.0.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fgutils"
-version = "0.0.7"
+version = "0.0.8"
 authors = [{name="Klaus Weinbauer", email="klaus@bioinf.uni-leipzig.de"}]
 description = "Library to get functional groups from molecular graphs."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `fgutils-0.0.7/PKG-INFO` & `fgutils-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fgutils
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library to get functional groups from molecular graphs.
 Project-URL: homepage, https://github.com/klausweinbauer/FGUtils
 Project-URL: source, https://github.com/klausweinbauer/FGUtils
 Project-URL: issues, https://github.com/klausweinbauer/FGUtils/issues
 Author-email: Klaus Weinbauer <klaus@bioinf.uni-leipzig.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

