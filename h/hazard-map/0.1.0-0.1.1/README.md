# Comparing `tmp/hazard_map-0.1.0.tar.gz` & `tmp/hazard_map-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazard_map-0.1.0.tar", max compression
+gzip compressed data, was "hazard_map-0.1.1.tar", max compression
```

## Comparing `hazard_map-0.1.0.tar` & `hazard_map-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      819 2024-04-08 12:54:07.269220 hazard_map-0.1.0/hazard_map/__init__.py
--rw-r--r--   0        0        0     6584 2024-04-08 14:58:41.040529 hazard_map-0.1.0/hazard_map/hazard_map.py
--rw-r--r--   0        0        0      429 2024-04-08 11:39:16.986546 hazard_map-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      432 2024-04-08 10:10:07.824482 hazard_map-0.1.0/readme.md
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 hazard_map-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      553 2024-04-15 13:44:28.900686 hazard_map-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      487 2024-04-15 13:45:26.090873 hazard_map-0.1.1/readme.md
+-rw-r--r--   0        0        0     1407 2024-04-15 13:46:33.681083 hazard_map-0.1.1/src/hazard_map/__init__.py
+-rw-r--r--   0        0        0     8737 2024-04-15 13:17:02.136480 hazard_map-0.1.1/src/hazard_map/hazard_map.py
+-rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 hazard_map-0.1.1/PKG-INFO
```

### Comparing `hazard_map-0.1.0/hazard_map/hazard_map.py` & `hazard_map-0.1.1/src/hazard_map/hazard_map.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 import networkx as nx
 from matplotlib import pyplot as plt
 
 
 @dataclass(frozen=True)
 class Sheet:
     name: str
+    id_list_locations: tuple[int, int]
+    name_list_locations: tuple[int, int]
+    mapping_table_location: tuple[int, int]
     transpose: bool
 
 class Kind(Enum):
     HAZARD = 'H'
     CAUSE = 'CA'
     CONTROL = 'CO'
 
-
 @dataclass(frozen=True)
 @functools.total_ordering
 class Node:
     kind: Kind
     number: int
 
     def to_str(self) -> str:
@@ -41,16 +43,15 @@
             int(match['number']),
         )
 
     def __lt__(self, other) -> bool:
         self.number < other.number
 
 
-OUTPUT_DIR = './output'
-if not os.path.exists('./output'): os.system(f'mkdir {OUTPUT_DIR}')
+DEFAULT_OUTPUT_DIR = './output'
 ZERO_PADDING_DIGITS = 2
 RENDERING_DPI = 480
 
 NODE_MATCHER = re.compile(r'^(?P<kind>H|CA|CO)-?(?P<number>\d+)$')
 MAPPING_MATCHER = re.compile('^\s*[Y]\s*$', re.I)
 
 KIND_STR_DICT = {
@@ -64,46 +65,81 @@
     Kind.CAUSE: '#7d5594',
     Kind.CONTROL: '#2762bc',
 }
 
 
 class HazardMap:
     def __init__(self, workbook_path: str):
-        self.WORKBOOK_NAME = self.parse_workbook_filename(workbook_path)
+        self.WORKBOOK_PATH = workbook_path
+        self.WORKBOOK_NAME = self.parse_workbook_filename(self.WORKBOOK_PATH)
 
         self.graph = nx.Graph()
 
     def parse_workbook_filename(self, workbook_path: str) -> str:
         workbook_filename = os.path.basename(workbook_path)
         workbook_filename_parts = workbook_filename.split('.')
         if workbook_filename_parts[-1] == 'xlsx': 
             return '.'.join(workbook_filename_parts[:-1])
         else:
             raise Exception('Please upload an xlsx file')
 
     def extract_sheet_mappings(self, sheets: list[Sheet]):
         for sheet in sheets:
-            df = pd.read_excel(self.WORKBOOK_NAME, sheet.name, index_col=0)
+            df = pd.read_excel(self.WORKBOOK_PATH, sheet.name, header=None, index_col=None)
+
+            # transform the sheet as appropriate
             if sheet.transpose: df = df.T
+            df = self._extract_clean_mappings(df, sheet)
 
             df.apply(self._extract_individual_mappings, axis=1)
 
+    def _extract_clean_mappings(self, df: pd.DataFrame, sheet: Sheet) -> pd.DataFrame:
+        # find out what size the mapping table is (i.e. how many pairs are in the table)
+        def find_list_length(s: pd.Series) -> int:
+            for i, item in enumerate(s): 
+                if item in [0, np.nan]: break
+            return i
+        table_dimensions = tuple([
+            find_list_length(name_list)
+            for name_list, axis in zip(
+                (
+                    df.iloc[sheet.name_list_locations[1], sheet.mapping_table_location[0]:], 
+                    df.iloc[sheet.mapping_table_location[1]:, sheet.name_list_locations[0]],
+                ),
+                ('horizontal', 'vertical'),
+            )
+        ])
+        # name the entries according to their labelling in the sheet
+        df = df.set_index(df.iloc[:, sheet.id_list_locations[1]])
+        df.columns = df.iloc[sheet.id_list_locations[0], :]
+        # reduce the dataframe to only the mappings on the sheet
+        df = df.iloc[
+            sheet.mapping_table_location[1]:sheet.mapping_table_location[1]+table_dimensions[1], 
+            sheet.mapping_table_location[0]:sheet.mapping_table_location[0]+table_dimensions[0],
+        ]
+        return df
+
     def _extract_individual_mappings(self, row: pd.Series):
         map_from = Node.from_str(row.name)
 
         row = row.dropna()
         mapped = row[row.str.match(MAPPING_MATCHER)].index.str.strip().to_list()
         mapped_typed = [Node.from_str(node_str) for node_str in mapped]
         
         for map_to in mapped_typed: self.graph.add_edge(map_from, map_to)
 
-    def write_to_file(self):
-        with pd.ExcelWriter(
-            f'{OUTPUT_DIR}/{self.WORKBOOK_NAME}-hazard_log_format.xlsx',
-        ) as writer:
+    def write_to_file(self, custom_output_location: str=None) -> str:
+        output_directory = (
+            custom_output_location if custom_output_location 
+            else DEFAULT_OUTPUT_DIR
+        )
+        if not os.path.exists(output_directory): os.system(f'mkdir {output_directory}')
+        output_file = f'{output_directory}/{self.WORKBOOK_NAME}-hazard_log_format.xlsx'
+        
+        with pd.ExcelWriter(output_file) as writer:
             for hazard in self.filter_node_set_for_kind(
                 self.graph.nodes, 
                 Kind.HAZARD,
             ):
                 cause_control_mappings = []
                 for cause in self.filter_node_set_for_kind(
                     self.graph[hazard], 
@@ -120,14 +156,16 @@
                         columns=['cause', 'control'],
                     )
                     .set_index('cause', append=True)
                     .reorder_levels([1, 0])
                     .to_excel(writer, sheet_name=hazard.to_str())
                 )
 
+        return output_file
+
     def filter_node_set_for_kind(self, node_set: set, kind: Kind) -> list[Node]:
         return sorted([node for node in node_set if node.kind == kind])
 
     def draw_graph(self) -> (plt.Figure, plt.Axes):        
         self.fig, self.ax = plt.subplots(
             frameon=False,
             figsize=(9, 7),
@@ -165,39 +203,47 @@
             min([
                 size_limits[0] + add_size_per_connect*n_connections,
                 size_limits[1],
             ])
             for node, n_connections in degrees
         ]
 
-    def save_graph(self): 
+    def save_graph(self, custom_output_location: str=None) -> str: 
         if not hasattr(self, 'fig'):
             self.draw_graph()
 
         filename = (
-            f'{OUTPUT_DIR}/{self.WORKBOOK_NAME}'
+            f'{self.WORKBOOK_NAME}'
             '-graph_rendering'
             f'-{str(hash(self.graph))[-4:]}'
             '.png'
         )
+        output_directory = (
+            custom_output_location if custom_output_location 
+            else DEFAULT_OUTPUT_DIR
+        )
+        if not os.path.exists(output_directory): os.system(f'mkdir {output_directory}')
+        output_file = f'{output_directory}/{self.WORKBOOK_NAME}-{filename}'
+
+        plt.savefig(output_file, transparent=True, dpi=RENDERING_DPI)
 
-        plt.savefig(filename, transparent=True, dpi=RENDERING_DPI)
+        return output_file
 
     def get_kind_connection_counts(self, kind: Kind) -> pd.DataFrame:
         comparison_kinds = [Kind.HAZARD, Kind.CAUSE, Kind.CONTROL]
         
         counts = [
             tuple([node.to_str()] + [
                     len(self.filter_node_set_for_kind(
                         self.graph.neighbors(node), 
                         comp_kind,
                     ))
                     for comp_kind in comparison_kinds
                 ])
-            for node in self.filter_node_set_for_kind(hazard_map.graph.nodes, kind)
+            for node in self.filter_node_set_for_kind(self.graph.nodes, kind)
         ]
             
         df = (
             pd.DataFrame(
                 data=counts, 
                 columns=['node'] + [kind.name.lower() for kind in comparison_kinds]
             )
@@ -208,8 +254,7 @@
         if len(df.columns) > 1:
             df['total'] = df.apply(np.sum, axis=1)
             df = df.sort_values('total', ascending=False)
         else:
             df = df.sort_values(df.columns[0], ascending=False)
             
         return df
-
```

### Comparing `hazard_map-0.1.0/PKG-INFO` & `hazard_map-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: hazard-map
-Version: 0.1.0
+Version: 0.1.1
 Summary: Build and analyze a network model of hazards, causes, and controls
+License: license.txt
 Author: Thom Cameron
 Author-email: thomcm@proton.me
 Requires-Python: >=3.11,<4.0
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: networkx (>=3.3,<4.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
     <h1>
         hazard-map
     </h1>
 </div>
 
-![screenshot](repo_assets/example_map.png)
+![screenshot](https://gitlab.com/thom-cameron/hazard-map/-/raw/main/repo_assets/example_map.png)
 
-Build a network model from spreadsheets of hazard, cause, and control mappings and carry out useful analyses 
+Build a network model from spreadsheets of hazard, cause, and control mappings and carry out useful analyses. 
 
 Overview
 --------
 
 This is a simple command-line tool that takes an Excel workbook with tables of mappings and creates a network model to use for analyses and visualization. 
 
 Installation
```

