# Comparing `tmp/witness-etl-0.0.8.tar.gz` & `tmp/witness_etl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "witness-etl-0.0.8.tar", last modified: Wed Dec 13 02:52:25 2023, max compression
+gzip compressed data, was "witness_etl-0.0.9.tar", last modified: Mon Apr 15 05:13:05 2024, max compression
```

## Comparing `witness-etl-0.0.8.tar` & `witness_etl-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-12-13 02:52:25.174575 witness-etl-0.0.8/
--rw-rw-rw-   0        0        0    11558 2022-04-10 07:08:20.000000 witness-etl-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1435 2023-12-13 02:52:25.174075 witness-etl-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-07-29 16:13:54.000000 witness-etl-0.0.8/README.md
--rw-rw-rw-   0        0        0      217 2022-06-24 13:23:37.000000 witness-etl-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0     1030 2023-12-13 02:52:25.175574 witness-etl-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-12-13 02:52:25.132576 witness-etl-0.0.8/witness/
--rw-rw-rw-   0        0        0      976 2023-07-29 16:13:54.000000 witness-etl-0.0.8/witness/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-13 02:52:25.141577 witness-etl-0.0.8/witness/core/
--rw-rw-rw-   0        0        0      712 2023-07-29 16:13:54.000000 witness-etl-0.0.8/witness/core/__init__.py
--rw-rw-rw-   0        0        0     4626 2023-11-29 08:43:22.000000 witness-etl-0.0.8/witness/core/abstract.py
--rw-rw-rw-   0        0        0     5857 2023-11-29 08:43:22.000000 witness-etl-0.0.8/witness/core/batch.py
--rw-rw-rw-   0        0        0     3307 2023-07-29 16:13:54.000000 witness-etl-0.0.8/witness/core/meta.py
-drwxrwxrwx   0        0        0        0 2023-12-13 02:52:25.150076 witness-etl-0.0.8/witness/extractors/
--rw-rw-rw-   0        0        0      632 2022-06-17 14:48:03.000000 witness-etl-0.0.8/witness/extractors/__init__.py
--rw-rw-rw-   0        0        0     2358 2023-07-29 16:13:54.000000 witness-etl-0.0.8/witness/extractors/database.py
--rw-rw-rw-   0        0        0      860 2023-07-29 16:13:54.000000 witness-etl-0.0.8/witness/extractors/file.py
--rw-rw-rw-   0        0        0     1252 2023-11-29 09:00:12.000000 witness-etl-0.0.8/witness/extractors/http.py
-drwxrwxrwx   0        0        0        0 2023-12-13 02:52:25.154076 witness-etl-0.0.8/witness/loaders/
--rw-rw-rw-   0        0        0      653 2023-11-29 08:43:22.000000 witness-etl-0.0.8/witness/loaders/__init__.py
--rw-rw-rw-   0        0        0     1333 2023-11-29 09:20:07.000000 witness-etl-0.0.8/witness/loaders/file.py
-drwxrwxrwx   0        0        0        0 2023-12-13 02:52:25.155077 witness-etl-0.0.8/witness/providers/
--rw-rw-rw-   0        0        0        0 2022-10-03 05:37:04.000000 witness-etl-0.0.8/witness/providers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-13 02:52:25.163575 witness-etl-0.0.8/witness/providers/pandas/
--rw-rw-rw-   0        0        0      630 2023-07-29 16:13:54.000000 witness-etl-0.0.8/witness/providers/pandas/__init__.py
--rw-rw-rw-   0        0        0     3295 2023-11-29 08:43:22.000000 witness-etl-0.0.8/witness/providers/pandas/core.py
--rw-rw-rw-   0        0        0     1500 2023-07-29 16:13:54.000000 witness-etl-0.0.8/witness/providers/pandas/extractors.py
--rw-rw-rw-   0        0        0     2922 2023-07-29 16:13:54.000000 witness-etl-0.0.8/witness/providers/pandas/loaders.py
-drwxrwxrwx   0        0        0        0 2023-12-13 02:52:25.167075 witness-etl-0.0.8/witness/serializers/
--rw-rw-rw-   0        0        0        0 2023-07-29 16:13:54.000000 witness-etl-0.0.8/witness/serializers/__init__.py
--rw-rw-rw-   0        0        0     1183 2023-11-29 09:08:48.000000 witness-etl-0.0.8/witness/serializers/common.py
--rw-rw-rw-   0        0        0      997 2023-07-29 16:13:54.000000 witness-etl-0.0.8/witness/version.py
-drwxrwxrwx   0        0        0        0 2023-12-13 02:52:25.173075 witness-etl-0.0.8/witness_etl.egg-info/
--rw-rw-rw-   0        0        0     1435 2023-12-13 02:52:25.000000 witness-etl-0.0.8/witness_etl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      753 2023-12-13 02:52:25.000000 witness-etl-0.0.8/witness_etl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-13 02:52:25.000000 witness-etl-0.0.8/witness_etl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2023-12-13 02:52:25.000000 witness-etl-0.0.8/witness_etl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-12-13 02:52:25.000000 witness-etl-0.0.8/witness_etl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 05:13:05.346679 witness_etl-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2022-10-24 01:46:22.000000 witness_etl-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1435 2024-04-15 05:13:05.345670 witness_etl-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2024-01-26 04:04:30.000000 witness_etl-0.0.9/README.md
+-rw-rw-rw-   0        0        0      217 2022-10-24 01:46:22.000000 witness_etl-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1030 2024-04-15 05:13:05.349674 witness_etl-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 05:13:05.300621 witness_etl-0.0.9/witness/
+-rw-rw-rw-   0        0        0      976 2024-01-26 04:04:30.000000 witness_etl-0.0.9/witness/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:13:05.306103 witness_etl-0.0.9/witness/core/
+-rw-rw-rw-   0        0        0      712 2024-01-26 04:04:30.000000 witness_etl-0.0.9/witness/core/__init__.py
+-rw-rw-rw-   0        0        0     4626 2024-01-26 04:05:13.000000 witness_etl-0.0.9/witness/core/abstract.py
+-rw-rw-rw-   0        0        0     5857 2024-01-26 04:05:13.000000 witness_etl-0.0.9/witness/core/batch.py
+-rw-rw-rw-   0        0        0     3307 2024-01-26 04:05:13.000000 witness_etl-0.0.9/witness/core/meta.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:13:05.311735 witness_etl-0.0.9/witness/extractors/
+-rw-rw-rw-   0        0        0      632 2022-10-24 01:46:22.000000 witness_etl-0.0.9/witness/extractors/__init__.py
+-rw-rw-rw-   0        0        0     2358 2024-01-26 04:04:30.000000 witness_etl-0.0.9/witness/extractors/database.py
+-rw-rw-rw-   0        0        0     1676 2024-03-07 16:35:33.000000 witness_etl-0.0.9/witness/extractors/file.py
+-rw-rw-rw-   0        0        0     1252 2024-01-26 04:05:13.000000 witness_etl-0.0.9/witness/extractors/http.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:13:05.314529 witness_etl-0.0.9/witness/loaders/
+-rw-rw-rw-   0        0        0      653 2024-01-26 04:05:13.000000 witness_etl-0.0.9/witness/loaders/__init__.py
+-rw-rw-rw-   0        0        0     2786 2024-04-10 02:13:15.000000 witness_etl-0.0.9/witness/loaders/file.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:13:05.316015 witness_etl-0.0.9/witness/providers/
+-rw-rw-rw-   0        0        0        0 2024-01-26 04:04:30.000000 witness_etl-0.0.9/witness/providers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:13:05.320925 witness_etl-0.0.9/witness/providers/pandas/
+-rw-rw-rw-   0        0        0      630 2024-01-26 04:04:30.000000 witness_etl-0.0.9/witness/providers/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3352 2024-04-10 03:42:14.000000 witness_etl-0.0.9/witness/providers/pandas/core.py
+-rw-rw-rw-   0        0        0     2816 2024-04-12 08:25:17.000000 witness_etl-0.0.9/witness/providers/pandas/extractors.py
+-rw-rw-rw-   0        0        0     3151 2024-04-10 03:42:14.000000 witness_etl-0.0.9/witness/providers/pandas/loaders.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:13:05.324391 witness_etl-0.0.9/witness/serializers/
+-rw-rw-rw-   0        0        0        0 2024-01-26 04:04:30.000000 witness_etl-0.0.9/witness/serializers/__init__.py
+-rw-rw-rw-   0        0        0     1183 2024-01-26 04:05:13.000000 witness_etl-0.0.9/witness/serializers/common.py
+-rw-rw-rw-   0        0        0      997 2024-04-12 05:09:50.000000 witness_etl-0.0.9/witness/version.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:13:05.343538 witness_etl-0.0.9/witness_etl.egg-info/
+-rw-rw-rw-   0        0        0     1435 2024-04-15 05:13:05.000000 witness_etl-0.0.9/witness_etl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      753 2024-04-15 05:13:05.000000 witness_etl-0.0.9/witness_etl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 05:13:05.000000 witness_etl-0.0.9/witness_etl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2024-04-15 05:13:05.000000 witness_etl-0.0.9/witness_etl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 05:13:05.000000 witness_etl-0.0.9/witness_etl.egg-info/top_level.txt
```

### Comparing `witness-etl-0.0.8/LICENSE` & `witness_etl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.8/PKG-INFO` & `witness_etl-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: witness-etl
-Version: 0.0.8
+Version: 0.0.9
 Summary: A minimal ETL library.
 Author: Eugene Popov
 Author-email: evgeniypalych@gmail.com
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/eppv/witness
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `witness-etl-0.0.8/README.md` & `witness_etl-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.8/setup.cfg` & `witness_etl-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6974 6e65 7373 2d65 746c 0d0a   = witness-etl..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 380d  version = 0.0.8.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 390d  version = 0.0.9.
 00000030: 0a61 7574 686f 7220 3d20 4575 6765 6e65  .author = Eugene
 00000040: 2050 6f70 6f76 0d0a 6175 7468 6f72 5f65   Popov..author_e
 00000050: 6d61 696c 203d 2065 7667 656e 6979 7061  mail = evgeniypa
 00000060: 6c79 6368 4067 6d61 696c 2e63 6f6d 0d0a  lych@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
 00000080: 6d69 6e69 6d61 6c20 4554 4c20 6c69 6272  minimal ETL libr
 00000090: 6172 792e 0d0a 6c6f 6e67 5f64 6573 6372  ary...long_descr
```

### Comparing `witness-etl-0.0.8/witness/__init__.py` & `witness_etl-0.0.9/witness/__init__.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.8/witness/core/__init__.py` & `witness_etl-0.0.9/witness/core/__init__.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.8/witness/core/abstract.py` & `witness_etl-0.0.9/witness/core/abstract.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.8/witness/core/batch.py` & `witness_etl-0.0.9/witness/core/batch.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.8/witness/core/meta.py` & `witness_etl-0.0.9/witness/core/meta.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.8/witness/extractors/__init__.py` & `witness_etl-0.0.9/witness/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.8/witness/extractors/database.py` & `witness_etl-0.0.9/witness/extractors/database.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.8/witness/extractors/http.py` & `witness_etl-0.0.9/witness/extractors/http.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.8/witness/loaders/__init__.py` & `witness_etl-0.0.9/witness/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.8/witness/providers/pandas/__init__.py` & `witness_etl-0.0.9/witness/providers/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.8/witness/providers/pandas/core.py` & `witness_etl-0.0.9/witness/providers/pandas/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,29 +41,29 @@
         elif isinstance(raw, dict):
             return self.handle_df_dict(raw)
         elif isinstance(raw, list):
             return self.handle_df_list(raw)
         else:
             raise ValueError("Unknown datastructure passed.")
 
-    def from_batch(self, data, *args, dtype="str", **kwargs):
+    def from_batch(self, data, *args, dtype: str = "str", **kwargs):
         df = pd.DataFrame(data, dtype=dtype)
         return df
 
 
 class PandasLoader(AbstractLoader):
     def __init__(
         self, uri, serializer: Optional[AbstractSerializer] = PandasSerializer()
     ):
         super().__init__(uri)
         self.serializer = serializer
 
-    def prepare(self, batch):
+    def prepare(self, batch, *args, dtype: str = "str", **kwargs):
         super().prepare(batch)
-        df = self.serializer.from_batch(batch.data)
+        df = self.serializer.from_batch(batch.data, dtype=dtype)
         self.output = df
         return self
 
     def attach_meta(self, meta_elements: Optional[list[str]] = None):
         super().attach_meta(meta_elements)
         for element in self.meta_to_attach:
             self.output[element] = self.meta_to_attach[element]
```

### Comparing `witness-etl-0.0.8/witness/providers/pandas/extractors.py` & `witness_etl-0.0.9/witness/providers/pandas/loaders.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,39 +8,88 @@
 #
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
+
+from witness.providers.pandas.core import PandasLoader
+from typing import Optional, Union
 import pandas as pd
-import logging
 
-from witness.providers.pandas.core import PandasExtractor
 
-log = logging.getLogger(__name__)
+class PandasSQLLoader(PandasLoader):
+    """
+    Loader that uses Pandas DataFrame.to_sql method for loading data.
+
+    :param engine: sqlalchemy engine;
+    :param table: name of the destination table;
+    :param schema: name of the destination schema, None if not defined.
+    """
+
+    def __init__(self,
+                 engine,
+                 table: str,
+                 schema: Optional[str] = None,
+                 method: Optional[str] = None,
+                 dtype: Union[str, dict, None] = None
+                 ):
+        self.engine = engine
+        self.schema = schema
+        self.table = table
+        self.method = method
+        self.dtype = dtype
+        uri = f"{schema}.{table}"
+        super().__init__(uri)
 
+    def load(self):
+        self.output.to_sql(
+            name=self.table,
+            con=self.engine,
+            schema=self.schema,
+            if_exists="append",
+            method=self.method,
+            dtype=self.dtype
+        )
+        return self
 
-class PandasFeatherExtractor(PandasExtractor):
-    def extract(self):
-        df = pd.read_feather(self.uri)
-        setattr(self, "output", df)
-        super().extract()
 
+class PandasExcelLoader(PandasLoader):
+    def __init__(self, uri, sheet_name="Sheet1", add_index=True):
+
+        self.sheet_name = sheet_name
+        self.add_index = add_index
+        super().__init__(uri)
+
+    def __load_single_sheet(self, **writer_kwargs):
+        with pd.ExcelWriter(path=self.uri, **writer_kwargs) as writer:
+            self.output.to_excel(
+                excel_writer=writer, sheet_name=self.sheet_name, index=self.add_index
+            )
         return self
 
+    def __load_multiple_sheets(self, **writer_kwargs):
+        with pd.ExcelWriter(path=self.uri, **writer_kwargs) as writer:
+            for sheet_name, df in self.output.items():
+                df.to_excel(
+                    excel_writer=writer,
+                    sheet_name=self.sheet_name,
+                    index=self.add_index,
+                )
+        return self
 
-class PandasExcelExtractor(PandasExtractor):
-    def __init__(self, uri, sheet_name=0, header=0, dtype=None):
-        self.sheet_name: str or int or None = sheet_name
-        self.header: int = header
-        self.dtype: str or dict or None = dtype
-        super().__init__(uri)
+    def load(self, **writer_kwargs):
+        if isinstance(self.output, pd.DataFrame):
+            return self.__load_single_sheet(**writer_kwargs)
+        elif isinstance(self.output, dict):
+            return self.__load_multiple_sheets(**writer_kwargs)
+        return self
 
-    def extract(self):
-        df = pd.read_excel(
-            self.uri, sheet_name=self.sheet_name, header=self.header, dtype=self.dtype
-        )
-        setattr(self, "output", df)
-        super().extract()
 
+class PandasFeatherLoader(PandasLoader):
+    def __init__(self, uri):
+        super().__init__(uri)
+
+    def load(self):
+        self.output.to_feather(self.uri)
         return self
```

### Comparing `witness-etl-0.0.8/witness/providers/pandas/loaders.py` & `witness_etl-0.0.9/witness/providers/pandas/extractors.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,81 +8,77 @@
 #
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
-
-from witness.providers.pandas.core import PandasLoader
 import pandas as pd
+import logging
+from typing import Optional, Union
+from witness.providers.pandas.core import PandasExtractor
+
+log = logging.getLogger(__name__)
 
 
-class PandasSQLLoader(PandasLoader):
-    """
-    Loader that uses Pandas DataFrame.to_sql method for loading data.
-
-    :param engine: sqlalchemy engine;
-    :param table: name of the destination table;
-    :param schema: name of the destination schema, None if not defined.
-    """
-
-    def __init__(
-        self, engine, table: str, schema: str or None = None, method: str or None = None
-    ):
-        self.engine = engine
-        self.schema = schema
-        self.table = table
-        self.method = method
-        uri = f"{schema}.{table}"
-        super().__init__(uri)
+class PandasFeatherExtractor(PandasExtractor):
+    def extract(self):
+        df = pd.read_feather(self.uri)
+        setattr(self, "output", df)
+        super().extract()
 
-    def load(self):
-        self.output.to_sql(
-            name=self.table,
-            con=self.engine,
-            schema=self.schema,
-            if_exists="append",
-            method=self.method,
-        )
         return self
 
 
-class PandasExcelLoader(PandasLoader):
-    def __init__(self, uri, sheet_name="Sheet1", add_index=True):
-
-        self.sheet_name = sheet_name
-        self.add_index = add_index
+class PandasExcelExtractor(PandasExtractor):
+    def __init__(self, uri, sheet_name=0, header=0, dtype=None):
+        self.sheet_name: str or int or None = sheet_name
+        self.header: int = header
+        self.dtype: str or dict or None = dtype
         super().__init__(uri)
 
-    def __load_single_sheet(self, **writer_kwargs):
-        with pd.ExcelWriter(path=self.uri, **writer_kwargs) as writer:
-            self.output.to_excel(
-                excel_writer=writer, sheet_name=self.sheet_name, index=self.add_index
-            )
-        return self
-
-    def __load_multiple_sheets(self, **writer_kwargs):
-        with pd.ExcelWriter(path=self.uri, **writer_kwargs) as writer:
-            for sheet_name, df in self.output.items():
-                df.to_excel(
-                    excel_writer=writer,
-                    sheet_name=self.sheet_name,
-                    index=self.add_index,
-                )
-        return self
+    def extract(self):
+        df = pd.read_excel(
+            self.uri, sheet_name=self.sheet_name, header=self.header, dtype=self.dtype
+        )
+        setattr(self, "output", df)
+        super().extract()
 
-    def load(self, **writer_kwargs):
-        if isinstance(self.output, pd.DataFrame):
-            return self.__load_single_sheet(**writer_kwargs)
-        elif isinstance(self.output, dict):
-            return self.__load_multiple_sheets(**writer_kwargs)
         return self
 
 
-class PandasFeatherLoader(PandasLoader):
-    def __init__(self, uri):
+class PandasSQLExtractor(PandasExtractor):
+    def __init__(self,
+                 engine,
+                 query: str,
+                 index_col: Optional[str] = None,
+                 params: Optional[dict] = None,
+                 table: Optional[str] = None,
+                 schema: Optional[str] = None,
+                 columns: Optional[list] = None,
+                 dtype: Union[str, dict, None] = None
+                 ):
+        self.engine = engine
+        self.query = query if query else table if table else 'select null'
+        self.index_col = index_col
+        self.params = params
+        self.schema = schema
+        self.table = table if self.schema is None else f'{self.schema}.{table}'
+        self.columns = columns
+        self.dtype = dtype
+        uri = f"{engine.url.database}.{schema}.{table}"
         super().__init__(uri)
 
-    def load(self):
-        self.output.to_feather(self.uri)
+    def extract(self):
+        conn = self.engine.connect()
+        df = pd.read_sql(
+            sql=self.query,
+            con=conn,
+            index_col=self.index_col,
+            params=self.params,
+            columns=self.columns,
+            # dtype=self.dtype only in pandas >= 2.0
+        )
+        setattr(self, "output", df)
+        super().extract()
+
         return self
```

### Comparing `witness-etl-0.0.8/witness/serializers/common.py` & `witness_etl-0.0.9/witness/serializers/common.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.8/witness/version.py` & `witness_etl-0.0.9/witness/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 except ImportError:
     from importlib import metadata  # type: ignore[no-redef]
 
 try:
     version = metadata.version('witness-etl')
 except metadata.PackageNotFoundError:
     import logging
-    version = '0.0.8'
+    version = '0.0.9'
 
 
 del metadata
 
 if __name__ == '__main__':
     print(version)
```

### Comparing `witness-etl-0.0.8/witness_etl.egg-info/PKG-INFO` & `witness_etl-0.0.9/witness_etl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: witness-etl
-Version: 0.0.8
+Version: 0.0.9
 Summary: A minimal ETL library.
 Author: Eugene Popov
 Author-email: evgeniypalych@gmail.com
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/eppv/witness
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `witness-etl-0.0.8/witness_etl.egg-info/SOURCES.txt` & `witness_etl-0.0.9/witness_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

