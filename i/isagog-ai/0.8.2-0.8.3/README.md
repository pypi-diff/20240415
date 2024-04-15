# Comparing `tmp/isagog_ai-0.8.2.tar.gz` & `tmp/isagog_ai-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isagog_ai-0.8.2.tar", max compression
+gzip compressed data, was "isagog_ai-0.8.3.tar", max compression
```

## Comparing `isagog_ai-0.8.2.tar` & `isagog_ai-0.8.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.8.2/isagog/__init__.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.8.2/isagog/client/__init__.py
--rw-r--r--   0        0        0     9306 2024-04-12 14:54:45.671149 isagog_ai-0.8.2/isagog/client/kg_client.py
--rw-r--r--   0        0        0     5971 2024-04-09 14:40:57.250758 isagog_ai-0.8.2/isagog/client/nlp_client.py
--rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.8.2/isagog/generator/__init__.py
--rw-r--r--   0        0        0     5838 2024-04-10 08:27:28.933122 isagog_ai-0.8.2/isagog/generator/sparql_generator.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.8.2/isagog/model/__init__.py
--rw-r--r--   0        0        0    16266 2024-04-12 15:51:09.197547 isagog_ai-0.8.2/isagog/model/kg_model.py
--rw-r--r--   0        0        0    27390 2024-04-10 09:06:24.629297 isagog_ai-0.8.2/isagog/model/kg_query.py
--rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.8.2/isagog/model/nlp_model.py
--rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.8.2/LICENSE
--rw-r--r--   0        0        0      588 2024-04-11 15:27:47.069933 isagog_ai-0.8.2/pyproject.toml
--rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.8.2/README.md
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.8.3/isagog/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.8.3/isagog/client/__init__.py
+-rw-r--r--   0        0        0     9327 2024-04-15 08:35:12.556546 isagog_ai-0.8.3/isagog/client/kg_client.py
+-rw-r--r--   0        0        0     5971 2024-04-09 14:40:57.250758 isagog_ai-0.8.3/isagog/client/nlp_client.py
+-rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.8.3/isagog/generator/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-10 08:27:28.933122 isagog_ai-0.8.3/isagog/generator/sparql_generator.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.8.3/isagog/model/__init__.py
+-rw-r--r--   0        0        0    18896 2024-04-15 11:50:48.729498 isagog_ai-0.8.3/isagog/model/kg_model.py
+-rw-r--r--   0        0        0    27390 2024-04-10 09:06:24.629297 isagog_ai-0.8.3/isagog/model/kg_query.py
+-rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.8.3/isagog/model/nlp_model.py
+-rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.8.3/LICENSE
+-rw-r--r--   0        0        0      588 2024-04-12 15:52:50.928459 isagog_ai-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.8.3/README.md
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.8.3/PKG-INFO
```

### Comparing `isagog_ai-0.8.2/isagog/client/kg_client.py` & `isagog_ai-0.8.3/isagog/client/kg_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import time
 from typing import Type, TypeVar
 
 # import requests
 import httpx
 from dotenv import load_dotenv
 
-from isagog.model.kg_model import Individual, Entity, Assertion, Ontology, Attribute, Concept, Relation, ID
+from isagog.model.kg_model import Individual, Entity, Assertion, Ontology, Attribute, Concept, Relation, Reference
 from isagog.model.kg_query import UnarySelectQuery, DisjunctiveClause, AtomicClause, Comparison, Value
 
 load_dotenv()
 
 KG_DEFAULT_TIMEOUT = int(os.getenv('KG_DEFAULT_TIMEOUT', 120))
 
 # Type variable for the Entity hierarchy
@@ -45,15 +45,15 @@
         self.dataset = dataset
         self.ontology = ontology
         self.version = version if version else "latest"
         self.logger = logger if logger else logging.getLogger()
         self.logger.info("Isagog KG client (%s) initialized on route %s", hex(id(self)), route)
 
     def get_entity(self,
-                   _id: ID,
+                   _id: Reference,
                    expand: bool = True,
                    entity_type: Type[E] = Entity
                    ) -> E | None:
         """
         Gets the entity by its identifier
         :param _id: the entity identifier
         :param expand: whether to return entity attributes
@@ -260,9 +260,9 @@
                     return False
             except Exception as e:
                 raise e
         else:
             self.logger.debug("Individual %s doesn't need update", individual.id)
 
 
-    def delete_individual(self, _id: ID, auth_key=None):
+    def delete_individual(self, _id: Reference, auth_key=None):
         pass
```

### Comparing `isagog_ai-0.8.2/isagog/client/nlp_client.py` & `isagog_ai-0.8.3/isagog/client/nlp_client.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.2/isagog/generator/sparql_generator.py` & `isagog_ai-0.8.3/isagog/generator/sparql_generator.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.2/isagog/model/kg_model.py` & `isagog_ai-0.8.3/isagog/model/kg_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
     A model for Knowledge Graph entities and relations
     (c) Isagog S.r.l. 2024, MIT License
 """
-import datetime
 import logging
-from typing import IO, TextIO, Any, Optional
+from typing import IO, TextIO, Any
 
 from rdflib import OWL, Graph, RDF, URIRef, RDFS
 
 # Type definitions
 
-ID = URIRef | str  # Identifier type
+Reference = URIRef | str
 
 OWL_ENTITY_TYPES = [OWL.Class, OWL.NamedIndividual, OWL.ObjectProperty, OWL.DatatypeProperty, OWL.AnnotationProperty]
 
 PROFILE_ATTRIBUTE = "https://isagog.com/ontology#profile"
 
 
 def _uri_label(uri: str) -> str:
@@ -56,29 +55,33 @@
     else:
         return obj
 
 
 class Entity(object):
     """
     Any identified knowledge entity, either predicative (property) or individual
+    Every entity has a string identifier and an optional meta type, which can be an OWL type
     """
 
-    def __init__(self, _id: ID, **kwargs):
+    def __init__(self, _id: Reference, **kwargs):
+        """
+
+        :param _id: the entity identifier, will be converted to a string
+        :param kwargs:
+        """
         assert _id
         self.id = str(_id).strip("<>")
         owl_type = kwargs.get('owl')
         if owl_type:
             if owl_type in OWL_ENTITY_TYPES:
-                self.__owl__ = owl_type
+                self.__meta__ = owl_type
             else:
                 logging.warning("bad owl type %s", owl_type)
-
-    def n3(self, namespace_manager: Optional["NamespaceManager"] = None) -> str:
-        """Convert to n3"""
-        return f"<{self.id}>"
+        else:
+            self.__meta__ = kwargs.get('meta', None)
 
     def __eq__(self, other):
         return (
                 (isinstance(other, Entity) and self.id == other.id)
                 or (isinstance(other, URIRef) and self.id == str(other).strip("<>"))
                 or (isinstance(other, str) and str(self.id) == other)
         )
@@ -86,29 +89,20 @@
     def __hash__(self):
         return self.id.__hash__()
 
     def to_dict(self) -> dict:
         return _todict(self)
 
 
-class Annotation(Entity):
-    """
-    References to owl:AnnotationProperty
-    """
-
-    def __init__(self, _id: ID, **kwargs):
-        super().__init__(self, _id=_id, owl=OWL.AnnotationProperty, **kwargs)
-
-
 class Concept(Entity):
     """
     Unary predicate
     """
 
-    def __init__(self, _id: ID, **kwargs):
+    def __init__(self, _id: Reference, **kwargs):
         """
 
         :param _id: the concept identifier
         :param kwargs:
         """
         super().__init__(_id, owl=OWL.Class, **kwargs)
         self.comment = kwargs.get('comment', "")
@@ -118,15 +112,15 @@
 
 class Attribute(Entity):
     """
     Assertions ranging on concrete domains
     owl:DatatypeProperties
     """
 
-    def __init__(self, _id: ID, **kwargs):
+    def __init__(self, _id: Reference, **kwargs):
         """
 
         :param _id:
         :param kwargs: domain
         """
 
         super().__init__(_id, owl=OWL.DatatypeProperty)
@@ -139,15 +133,15 @@
     """
     Assertions ranging on individuals
     owl:ObjectProperty
     """
 
     def __init__(
             self,
-            _id: ID,
+            _id: Reference,
             **kwargs
     ):
         """
         :param _id:
         :param kwargs: inverse, domain, range, label
         """
 
@@ -161,45 +155,40 @@
 
 class Assertion(object):
     """
     Assertion axiom of the form: property(subject, values)
     """
 
     def __init__(self,
-                 predicate: ID = None,
-                 subject: ID = None,
+                 predicate: Reference = None,
+                 subject: Reference = None,
                  values: list = None,
                  **kwargs):
         """
 
         :param predicate:
         :param subject:
         :param values:
         """
         if predicate is None:
+            # try to get the predicate from the kwargs, if not present raise an error
             predicate = kwargs.get('property', kwargs.get('id', None))
             if predicate is None:
                 raise ValueError("missing predicate")
-        if values is None:
-            values = kwargs.get('values', [])
 
         self.predicate = str(predicate).strip("<>")
         self.subject = str(subject).strip("<>") if subject else None
         self.values = values if values else []
 
-    def n3(self, namespace_manager: Optional["NamespaceManager"] = None) -> list[str]:
-        """Convert to n3"""
-        rt = []
-        for value in self.values:
-            rt.append(f"<{self.subject}> <{self.predicate}> {value}")
-        return rt
-
     def to_dict(self) -> dict:
         return _todict(self)
 
+    def is_empty(self) -> bool:
+        return not self.values
+
 
 class Ontology(Graph):
     """
     In-memory, read-only RDF representation of an ontology.
     Manages basic reasoning on declared inclusion dependencies (RDFS.subClassOf).
     Also, it manages classes annotated as 'category' in the ontology. Categories
     are 'rigid' concepts,
@@ -288,78 +277,119 @@
 
 
 class AttributeInstance(Assertion):
     """
     Attributive assertion
     """
 
-    def __init__(self, predicate: ID = None,
-                 subject: ID = None,
-                 values: list = None,
+    def __init__(self, predicate: Reference = None,
+                 subject: Reference = None,
+                 values: list[str | int | float | bool] = None,
                  **kwargs):
         """
         :param subject: the asserted subject
         :param predicate: the asserted property
-        :param values: the asserted values
+        :param values: the asserted values, they can be strings, integers, floats or booleans
         :param kwargs:
         """
-
+        self.value_type = kwargs.get('type')
+        if values:
+            specimen = values[0]
+            if isinstance(specimen, str):
+                if self.value_type:
+                    if self.value_type == "string":
+                        pass
+                    else:
+                        raise ValueError("bad values for string attribute")
+                else:
+                    self.value_type = "string"
+
+            elif isinstance(specimen, int):
+                if self.value_type:
+                    if self.value_type == "int":
+                        pass
+                    else:
+                        raise ValueError("bad values for int attribute")
+                else:
+                    self.value_type = "int"
+                raise ValueError("bad values for int attribute")
+
+            elif isinstance(specimen, float):
+                if self.value_type:
+                    if self.value_type == "float":
+                        pass
+                    else:
+                        raise ValueError("bad values for float attribute")
+                else:
+                    self.value_type = "float"
+
+            elif isinstance(specimen, bool):
+                if self.value_type:
+                    if self.value_type == "bool":
+                        pass
+                    else:
+                        raise ValueError("bad values for bool attribute")
+                else:
+                    self.value_type = "bool"
+            else:
+                raise ValueError("bad values for attribute")
         super().__init__(predicate=predicate,
                          subject=subject,
                          values=values,
                          **kwargs)
-        self.value_type = kwargs.get('type', "string")
 
     def all_values_as_string(self) -> str:
         match len(self.values):
             case 0:
                 return ""
             case 1:
-                return self.values[0]
+                return str(self.values[0])
             case _:
-                return "\n".join(self.values)
+                return "\n".join([str(v) for v in self.values])
 
     def all_values(self) -> list:
         return self.values
 
-    def first_value(self, default=None) -> Any | None:
+    def first_value(self, default=None) -> str | int | float | bool | None:
         if len(self.values) > 0:
             return self.values[0]
         else:
             return default
 
-    def is_empty(self) -> bool:
-        return len(self.values) == 0 or self.values[0] == "None"
-
 
 VOID_ATTRIBUTE = AttributeInstance(predicate='http://isagog.com/attribute#void')
 
 
 class RelationInstance(Assertion):
     """
     Relational assertion
     """
 
-    def __init__(self, predicate: ID = None, subject: ID = None, values: list = None, **kwargs):
+    def __init__(self, predicate: Reference = None,
+                 subject: Reference = None,
+                 values: list[Any | Reference | dict] = None,
+                 **kwargs):
         """
 
         :param property: the asserted property
         :param subject: the assertion's subject
-        :param values: the asserted values
+        :param values: the asserted values, they can be individuals, references or dictionaries
         :param kwargs:
         """
         if values:
             specimen = values[0]
-            if isinstance(specimen, Individual):
+            if isinstance(specimen, (Individual, Reference)):
+                # values are acceptable
                 pass
             elif isinstance(specimen, dict):
+                # if values are dictionaries, then convert them to Individuals
                 inst_values = [Individual(_id=r_data.get('id'), **r_data) for r_data in values]
                 values = inst_values
             else:
-                raise ValueError("bad values for relation instance")
+                raise ValueError("bad values for relational assertion")
         super().__init__(predicate=predicate,
                          subject=subject,
                          values=values,
                          **kwargs)
 
     def all_values(self, only_id=True) -> list:
         """
@@ -377,17 +407,14 @@
             if only_id:
                 return self.values[0].id
             else:
                 return self.values[0]
         else:
             return default
 
-    def is_empty(self) -> bool:
-        return len(self.values) == 0
-
     def kind_map(self) -> dict:
         """
         Returns a map of individuals by kind
         :return: a map of kind : individuals
         """
         kind_map = {}
         for individual in self.values:
@@ -403,80 +430,96 @@
 
 class Individual(Entity):
     """
     Individual entity
 
     """
 
-    def __init__(self, _id: ID, **kwargs):
+    def __init__(self, _id: Reference,
+                 attributes: list[AttributeInstance | dict] = None,
+                 relations: list[RelationInstance | dict] = None,
+                 **kwargs):
         """
 
         :param _id: the individual identifier
+        :param attributes: the individual attributes
+        :param relations: the individual relations
         :param kwargs:
         """
         super().__init__(_id, owl=OWL.NamedIndividual, **kwargs)
         self.attributes = []
         self.relations = []
-        self.label = kwargs.get('label', _uri_label(self.id))
-        self.add_attribute(AttributeInstance(predicate=RDFS.label, values=[self.label]))
-
-        self.kind = kwargs.get('kind', kwargs.get('kinds', [OWL.Thing]))  # back compatibility w 0.7
-        if not all(x == OWL.Thing for x in self.kind):
-            self.add_attribute(AttributeInstance(predicate=RDF.type, values=self.kind))
-
-        self.comment = kwargs.get('comment', '')
-        if self.comment:
-            self.add_attribute(AttributeInstance(predicate=RDFS.comment, values=[self.comment]))
-
-        self.attributes.extend([AttributeInstance(**a_data) for a_data in
-                                kwargs.get('attributes', list[AttributeInstance]())])
-        self.relations.extend(
-            [RelationInstance(**r_data) for r_data in kwargs.get('relations', list[RelationInstance]())])
+        # self.label = kwargs.get('label', _uri_label(self.id))
+        # self.add_attribute(AttributeInstance(predicate=RDFS.label, values=[self.label]))
+        #
+        # self.kind = kwargs.get('kind', kwargs.get('kinds', [OWL.Thing]))  # back compatibility w 0.7
+        # if not all(x == OWL.Thing for x in self.kind):
+        #     self.add_attribute(AttributeInstance(predicate=RDF.type, values=self.kind))
+        #
+        # self.comment = kwargs.get('comment', '')
+        # if self.comment:
+        #     self.add_attribute(AttributeInstance(predicate=RDFS.comment, values=[self.comment]))
+
+        if attributes:
+            for attribute in attributes:
+                if isinstance(attribute, dict):
+                    attribute = AttributeInstance(**attribute)
+                self.add_attribute(attribute)
+
+        # self.attributes.extend([AttributeInstance(**a_data) for a_data in
+        #                         kwargs.get('attributes', list[AttributeInstance]())])
+        if relations:
+            for relation in relations:
+                if isinstance(relation, dict):
+                    relation = RelationInstance(**relation)
+                self.add_relation(relation)
+        # self.relations.extend(
+        #     [RelationInstance(**r_data) for r_data in kwargs.get('relations', list[RelationInstance]())])
         if 'score' in kwargs:
             self.score = float(kwargs.get('score'))
         if self.has_attribute(PROFILE_ATTRIBUTE):
             self.profile = {
                 profile_value.split("=")[0]: int(profile_value.split("=")[1])
                 for profile_value in self.get_attribute(PROFILE_ATTRIBUTE).values
             }
         else:
             self.profile = {}
         self._refresh = True
 
-    def has_attribute(self, attribute_id: ID) -> bool:
+    def has_attribute(self, attribute_id: Reference) -> bool:
         """
         Checks if the individual has a given ontology defined attribute
         :param attribute_id:
         :return:
         """
         found = next(filter(lambda x: x.predicate == attribute_id, self.attributes), None)
         return found and not found.is_empty()
 
-    def get_attribute(self, attribute_id: ID) -> AttributeInstance | Any:
+    def get_attribute(self, attribute_id: Reference) -> AttributeInstance | None:
         """
         Gets the ontology defined attribute instance of the individual
         :param attribute_id:
         :return:
         """
         found = next(filter(lambda x: x.predicate == attribute_id, self.attributes), None)
         if found and not found.is_empty():
             return found
         else:
             return VOID_ATTRIBUTE
 
-    def has_relation(self, relation_id: ID) -> bool:
+    def has_relation(self, relation_id: Reference) -> bool:
         """
         Checks if the individual has a given ontology defined relation
         :param relation_id:
         :return:
         """
         found = next(filter(lambda x: x.predicate == relation_id, self.relations), None)
         return found and not found.is_empty()
 
-    def get_relation(self, relation_id: ID) -> RelationInstance | Any:
+    def get_relation(self, relation_id: Reference) -> RelationInstance | None:
         """
         Gets the ontology defined relation instance of the individual
         :param relation_id:
         :return:
         """
         found = next(filter(lambda x: x.predicate == relation_id, self.relations), None)
         if found and not found.is_empty():
@@ -504,24 +547,28 @@
         return hasattr(self, 'score')
 
     def add_attribute(self, attribute: AttributeInstance):
         """
         Adds an attribute to the individual
         :param attribute:
         """
+        if attribute.subject and attribute.subject != self.id:
+            logging.warning("attribute for %s redeclared for %s", attribute.subject, self.id)
         attribute.subject = self.id
         self.attributes.append(attribute)
         self._refresh = True
 
     def add_relation(self, relation: RelationInstance):
         """
 
         :param relation:
         :return:
         """
+        if relation.subject and relation.subject != self.id:
+            logging.warning("relation for %s redeclared for %s", relation.subject, self.id)
         relation.subject = self.id
         self.relations.append(relation)
         self._refresh = True
 
     def need_update(self):
         return self._refresh
```

### Comparing `isagog_ai-0.8.2/isagog/model/kg_query.py` & `isagog_ai-0.8.3/isagog/model/kg_query.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.2/LICENSE` & `isagog_ai-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.2/pyproject.toml` & `isagog_ai-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2269 7361 676f 672d 6169  ame = "isagog-ai
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 302e  "..version = "0.
-00000030: 382e 3222 0d0a 6465 7363 7269 7074 696f  8.2"..descriptio
+00000030: 382e 3322 0d0a 6465 7363 7269 7074 696f  8.3"..descriptio
 00000040: 6e20 3d20 2263 6c69 656e 7420 666f 7220  n = "client for 
 00000050: 6973 6167 6f67 2061 6920 7365 7276 6963  isagog ai servic
 00000060: 6573 220d 0a61 7574 686f 7273 203d 205b  es"..authors = [
 00000070: 2247 7569 646f 2056 6574 6572 6520 3c67  "Guido Vetere <g
 00000080: 2e76 6574 6572 6540 6973 6167 6f67 2e63  .vetere@isagog.c
 00000090: 6f6d 3e22 5d0d 0a72 6561 646d 6520 3d20  om>"]..readme = 
 000000a0: 2252 4541 444d 452e 6d64 220d 0a70 6163  "README.md"..pac
```

### Comparing `isagog_ai-0.8.2/PKG-INFO` & `isagog_ai-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isagog-ai
-Version: 0.8.2
+Version: 0.8.3
 Summary: client for isagog ai services
 Author: Guido Vetere
 Author-email: g.vetere@isagog.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

