# Comparing `tmp/pypomes_core-0.8.4.tar.gz` & `tmp/pypomes_core-0.8.5.tar.gz`

## Comparing `pypomes_core-0.8.4.tar` & `pypomes_core-0.8.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    23119 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27941 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    23119 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/PKG-INFO
```

### Comparing `pypomes_core-0.8.4/src/pypomes_core/.ruff.toml` & `pypomes_core-0.8.5/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.4/src/pypomes_core/__init__.py` & `pypomes_core-0.8.5/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.4/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.8.5/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.4/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.8.5/src/pypomes_core/dict_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -218,15 +218,15 @@
             result = parent.pop(key)
 
     return result
 
 
 def dict_replace_value(target: dict, old_value: any, new_value: any) -> None:
     """
-    Replace in *target* all occurrences of *old_value* with *new_value*.
+    Replace, in *target*, all occurrences of *old_value* with *new_value*.
 
     :param target: the reference dict
     :param old_value: the value to be replaced
     :param new_value: the new value
     """
     def list_replace_value(items: list[any], old_val: any, new_val: any) -> None:
         # traverse the list
@@ -426,21 +426,21 @@
 
         # replace the original list with the coalesced new list
         curr_dict[key_chain[-2]] = penultimate_list
 
 
 def dict_reduce(target: dict, key_chain: list[str]) -> None:
     """
-    Realoca os elementos de *target* no nível *n*, para o nível imediatamente acima.
+    Relocate the elements from *target* at level *n*, to the level immediately above.
 
-    Esses elementos são apontados pela cadeia de chaves aninhadas *[keys[0]: ... :keys[n]*.
-    O elemento no nivel *n* é removido, ao final.
+    These elements are pointed to by the nested key chain *[keys[0]: ... :keys[n]*.
+    The element at level *n* is removed at the end.
 
-    :param target: o dicionário a ser reduzido
-    :param key_chain: a cadeia de chaves
+    :param target: the 'dict' to be reduced
+    :param key_chain: the key chain
     """
     # a cadeia de chaves contem pelo menos 1 chave ?
     if len(key_chain) > 0:
         # sim, prossiga
 
         curr_dict: dict | None = target
         # percorre a cadeia até a penúltima chave
@@ -475,98 +475,99 @@
             last: dict = curr_dict.pop(last_key)
             for key, value in last.items():
                 curr_dict[key] = value
 
 
 def dict_from_list(source: list[dict], key_chain: list[str], value: any) -> dict:
     """
-    Localiza em *source*, e retorna, o elemento do tipo *dict* com o valor *value* na cadeia de chaves *key_chain*.
+    Locate in *source*, and return, the element of type *dict* with value *value* in the key chain *key_chain*.
 
-    Retorna *None* se esse *dict* não for encontrado.
-
-    :param source: a lista a ser inspecionada
-    :param key_chain: a cadeia de chaves usada na busca
-    :param value: o valor associado à cadeia de chaves
-    :return: o dict procurado
+    :param source: the list to be inspected
+    :param key_chain: the key chain used in the search process
+    :param value: the value of the element pointed to by the key chain
+    :return: the 'dict' wanted, or 'None' if not found
     """
-    # inicializa a variável de retorno
+    # initialize the return variable
     result: dict | None = None
 
     for item in source:
         if isinstance(item, dict) and \
            value == dict_get_value(item, key_chain):
             result = item
             break
 
     return result
 
 
 def dict_from_object(source: object) -> dict:
     """
-    Percorre *source* e cria um *dict* com seus atributos contendo valores não nulos.
+    Create a *dict* and populate it with the attributes in *source* containing non-None values.
 
-    *source* pode ser qualquer objeto, especialmente aqueles que tenham sido decorados com *@dataclass*.
+    The input *source* might be any *object*, specially those decorated with *@dataclass*.
 
-    :param source: o objeto de referência
-    :return: dicionário com estrutura equivalente ao objeto de referência
+    :param source: the reference object
+    :return: 'dict' structurally similar to the reference object
     """
-    # inicializa a variável de retorno
+    # initialize the return variable
     result: dict = {}
 
+    # obtain the object's source module
     source_module: types.ModuleType = inspect.getmodule(source)
+    # obtain the source module's dictionary
     source_dict: dict = source.__dict__
+    # traverse it
     for key, value in source_dict.items():
-        # value é nulo ou lista vazia ?
+        # is 'value' None or an empty list ?
         if not (value is None or (isinstance(value, list) and len(value) == 0)):
-            # não, prossiga
+            # no, proceed
             name: str = key
 
-            # value é uma lista ?
+            # is 'value' a list ?
             if isinstance(value, list):
-                # sim, percorra-a
+                # es, traverse it
                 result[name] = []
                 for list_item in value:
-                    # list_item é um objeto do mesmo módulo ?
+                    # is 'list_item' an object of the same module ?
                     if source_module == inspect.getmodule(list_item):
-                        # sim, prossiga recursivamente
+                        # yes, proceed recursively
                         result[name].append(dict_from_object(list_item))
                     else:
-                        # não, prossiga linearmente
+                        # no, proceed linearly
                         result[name].append(list_item)
 
-            # value é um objeto do mesmo módulo ?
+            # is 'value' an object of the same module ?
             elif source_module == inspect.getmodule(value):
-                # sim, prossiga recursivamente
+                # yes, proceed recursively
                 result[name] = dict_from_object(value)
             else:
-                # não, prossiga linearmente
+                # no, proceed linearly
                 result[name] = value
 
     return result
 
 
 def dict_transform(source: dict, from_to_keys: list[tuple[str, str]],
                    prefix_from: str = None, prefix_to: str = None) -> dict:
     """
-    Constrói um novo *dict*, segundo as regras seguintes.
+    Build a new *dict*, according to the rules presented herein.
 
-    Esse dicionário é construído criando-se, para cada elemento da lista de tuplas em
-    *from_to_keys*, o elemento indicado pelo segundo termo da tupla, atribuindo-se a ele
-    o valor do elemento de *source* indicado pelo primeiro termo da tupla. Ambos os termos
-    das tuplas são representados por uma cadeia de chaves aninhadas.
-
-    Os prefixos para as chaves de origem e de destino, se definidos, tem tratamentos distintos.
-    São acrescentados na busca de valores em *Source*, e removidos na atribuição de valores
-    ao *dict* de retorno.
-
-    :param source: o dict de origem dos valores
-    :param from_to_keys: a lista de tuplas contendo as sequências de chaves de origem e destino
-    :param prefix_from: prefixo a ser acrescentado às chaves de origem
-    :param prefix_to: prefixo a ser removido das chaves de destino
-    :return: o novo dicionário
+    This dictionary is constructed by creating, for each element of the list of tuples in
+    *from_to_keys*, the element indicated by the second term of the tuple, assigning to it
+    the value of the *source* element indicated by the first term of the tuple. Both terms
+    of the tuples are represented by a chain of nested keys.
+
+    The prefixes for the source and destination keys, if defined, have fferent treatments.
+    They are added when searching for values in *Source*, and removed when assigning values
+    to the return *dict*.
+
+    :param source: the source 'dict' of the values
+    :param from_to_keys: the list of tuples containing the source and destination key sequences
+    :param prefix_from: prefix to be added to source keys
+    :param prefix_to: prefix to be removed from target keys
+    :return: the new 'dict'
     """
     # import the neeeded functions
     from .list_pomes import list_find_coupled, list_transform, list_unflatten
 
     # inicializa a variável de retorno
     result: dict = {}
```

### Comparing `pypomes_core-0.8.4/src/pypomes_core/email_pomes.py` & `pypomes_core-0.8.5/src/pypomes_core/email_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 EMAIL_PORT: Final[int] = env_get_int(f"{APP_PREFIX}_EMAIL_PORT")
 EMAIL_SERVER: Final[str] = env_get_str(f"{APP_PREFIX}_EMAIL_SERVER")
 
 
 def email_send(errors: list[str] | None, user_email: str,
                subject: str, content: str, logger: Logger = None) -> None:
     """
-    Send email, to *user_email", with *subject* as the email subject, and *content* as the email message.
+    Send email to *user_email", with *subject* as the email subject, and *content* as the email message.
 
     :param errors: incidental error messages
     :param user_email: the address to send the email to
     :param subject: the email subject
     :param content: the email message
     :param logger: optional logger
     """
```

### Comparing `pypomes_core-0.8.4/src/pypomes_core/env_pomes.py` & `pypomes_core-0.8.5/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.4/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.8.5/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.4/src/pypomes_core/file_pomes.py` & `pypomes_core-0.8.5/src/pypomes_core/file_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,29 +38,29 @@
             result: bytes = file.stream.read()
 
     return result
 
 
 def file_get_data(file_data: Path | str | bytes) -> bytes:
     """
-    Retrieve and return the data in *file_data* (typeipo *bytes*), or in a file in path *file_data* (tipo *str*).
+    Retrieve and return the data in *file_data* (typeipo *bytes*), or in a file in path *file_data* (type *str*).
 
     :param file_data: file data, or the path to locate the file
     :return: the data
     """
     # declare the return variable
     result: bytes
 
     # what is the argument type ?
     if isinstance(file_data, bytes):
         # argument is type 'bytes'
         result = file_data
 
     else:  # isinstance(file_data, Path) or isinstance(file_data, str)
-        # argumento is a file path
+        # argument is a file path
         buf_size: int = 128 * 1024
         file_path: Path = file_data if isinstance(file_data, Path) else Path(file_data)
         with file_path.open("rb") as f:
             file_bytes: bytearray = bytearray()
             while True:
                 in_bytes: bytes = f.read(buf_size)
                 if in_bytes:
```

### Comparing `pypomes_core-0.8.4/src/pypomes_core/json_pomes.py` & `pypomes_core-0.8.5/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.4/src/pypomes_core/list_pomes.py` & `pypomes_core-0.8.5/src/pypomes_core/list_pomes.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,143 +25,143 @@
         result = False
 
     return result
 
 
 def list_flatten(source: list[str]) -> str:
     """
-    Transforma uma lista de *str* em uma *str* consistindo na concatenação com "." dos elementos da lista.
+    Buiild and return a *str* by concatenating with "." the elements in *source*.
 
-    Exemplos:
+    Exemples:
         - ['1', '2', '']     -> '1.2.'
         - ['', 'a', 'b']     -> '.a.b'
         - ['x', '', '', 'y'] -> 'x...y'
         - ['z']              -> 'z'
 
-    :param source: a lista de strings
-    :return: a string concatenada
+    :param source: the source list
+    :return: the concatenated elements of the source list
     """
     result: str = ""
     for item in source:
         result += "." + item
     return result[1:]
 
 
 def list_unflatten(source: str) -> list[str]:
     """
-    Transforma uma *str* contendo elementos concatenados por "." em uma lista de *str*.
+    Build and return a *list*, by splitting *source* into its components separated by ".".
 
-    Essa lista contem os sub_elementos extraídos. Exemplos:
+    This *list* will contain the extracted components. Exemples:
         - '1.2.'  -> ['1', '2', '']
         - '.a.b'  -> ['', 'a', 'b']
         - 'x...y' -> ['x', '', '', 'y']
         - 'z'     -> ['z']
 
-    :param source: string com elementos concatenados por "."
-    :return: a lista de strings contendo os elementos da concatenação
+    :param source: string with components concatenated by "."
+    :return: the list of strings containing the concatenated components
     """
     # import the needed function
     from .str_pomes import str_split_on_mark
 
     return str_split_on_mark(source, ".")
 
 
 def list_find_coupled(coupled_elements: list[tuple[str, str]], primary_element: str) -> str:
     """
-    Localiza em *coupled_elements* o elemento acoplado ao *primary_element* dado.
+    Locate in *coupled_elements*, and return, the element coupled to *primary_element*.
 
-    Se *primary_element* contiver indicação de índice (denotado por *[<pos>]*), essa indicação é removida.
-    Essa função é utilizada na transformação de *dicts* (*dict_transform*) e *lists* (*list_transform*),
-    a partir de sequências de pares de chaves.
+    If *primary_element* contains an index indication (denoted by *[<pos>]*), this indication is removed.
+    This function is used in the transformation of *dicts* (*dict_transform*) and *lists* (*list_transform*),
+    from sequences of key pairs.
 
-    :param coupled_elements: a lista de tuplas contendo os pares de elementos.
-    :param primary_element: o elemento primário
-    :return: o elemento acoplado, ou None se não for encontrado
+    :param coupled_elements: list of tupl4s containing the pairs of elements
+    :param primary_element: the primary element
+    :return: the couple element, or 'None' if it is not foundo
     """
-    # remove a indicação de elemento de lista
+    # initialize the return variable
+    result: str | None = None
+
+    # remove the list element indication
     pos1: int = primary_element.find("[")
     while pos1 > 0:
         pos2: int = primary_element.find("]", pos1)
         primary_element = primary_element[:pos1] + primary_element[pos2+1:]
         pos1 = primary_element.find("[")
 
-    # inicializa a variável de retorno
-    result: str | None = None
-
-    # percorre a list de elementos acoplados
+    # traverse the list of coupled elements
     for primary, coupled in coupled_elements:
-        # o elemento primário foi encontrado ?
+        # has the primary element been found ?
         if primary == primary_element:
-            # sim, retorne o elemento acoplado correspondente
+            # yes, return the corresponding coupled element
             result = coupled
             break
 
     return result
 
 
 def list_transform(source: list[any], from_to_keys: list[tuple[str, str]],
                    prefix_from: str = None, prefix_to: str = None) -> list[any]:
     """
-    Constrói uma nova *list*, transformando elementos do tipo *list* e *dict* encontrados em *source*.
+    Construct a new *list*, transforming elements of type *list* and *dict* found in *source*.
 
-    A conversão dos elementos tipo *dict* está documentada na função *dict_transform*.
+    The conversion of *dict* type elements is documented in the *dict_transform* function.
 
-    Os prefixos para as chaves de origem e de destino, se definidos, tem tratamentos distintos.
-    São acrescentados na busca de valores em *Source*, e removidos na atribuição de valores
-    ao *dict* de retorno.
-
-    :param source: o dict de origem dos valores
-    :param from_to_keys: a lista de tuplas contendo as sequências de chaves de origem e destino
-    :param prefix_from: prefixo a ser acrescentado às chaves de origem
-    :param prefix_to: prefixo a ser removido das chaves de destino
-    :return: a nova lista
+    The prefixes for the source and destination keys, if defined, have different treatments.
+    They are added when searching for values in *Source*, and removed when assigning values
+    to the return *dict*.
+
+    :param source: the source 'dict' of the values
+    :param from_to_keys: the list of tuples containing the source and destination key sequences
+    :param prefix_from: prefix to be added to the source keys
+    :param prefix_to: prefix to be removed from the target keys
+    :return: the new list
     """
     # import the needed function
     from .dict_pomes import dict_transform
 
-    # inicializa a variável de retorno
+    # initialize the return variable
     result: list[any] = []
 
-    # percorre a lista de origem
+    # traverse the source list
     for inx, value in enumerate(source):
         if prefix_from is None:
             from_keys: None = None
         else:
             from_keys: str = f"{prefix_from}[{inx}]"
 
-        # obtem o valor de destino
+        # obtain the target value
         if isinstance(value, dict):
             to_value: dict = dict_transform(value, from_to_keys, from_keys, prefix_to)
         elif isinstance(value, list):
             to_value: list = list_transform(value, from_to_keys, from_keys, prefix_to)
         else:
             to_value: any = value
 
-        # acrescenta o valor transformado ao resultado
+        # added the value transformed to 'result'
         result.append(to_value)
 
     return result
 
 
 def list_elem_starting_with(source: list[str | bytes],
                             prefix: str | bytes, keep_prefix: bool = True) -> str | bytes:
     """
-    Localiza e retorna o primeiro elemento em *source* prefixado por *prefix*.
+    Locate and return the first element in *source* prefixed by *prefix*.
 
     Retorna *None* se esse elemento não for encontrado.
 
-    :param source: a lista a ser inspecionada
-    :param prefix: o dado prefixando o elemento a ser retornado
-    :param keep_prefix: define se o elemento encontrado deve ou não ser retornado com o prefixo
-    :return: o elemento prefixado, com ou sem o prefixo
+    :param source: the list to be inspected
+    :param prefix: the data prefixing the element to be returned
+    :param keep_prefix: defines whether or not the found element should be returned with the prefix
+    :return: the prefixed element, with or without the prefix, or 'None' if not found
     """
-    # inicializa a variável de retorno
+    # initialize the return variable
     result: str | bytes | None = None
 
-    # percorre a lista de origem
+    # traverse the source list
     for elem in source:
         if elem.startswith(prefix):
             if keep_prefix:
                 result = elem
             else:
                 result = elem[len(prefix)+1:]
             break
```

### Comparing `pypomes_core-0.8.4/src/pypomes_core/str_pomes.py` & `pypomes_core-0.8.5/src/pypomes_core/str_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,18 +49,18 @@
 def str_find_whitespace(source: str) -> int:
     """
     Locate and return the position of the first occurence of a *whitespace* character in *source*.
 
     :param source: the string to be inspected
     :return: the position of the first whitespace character, or -1 if none was found
     """
-    # inicializa a variável de retorno
+    # initialize the return variable
     result: int = -1
 
-    # busca por whitespace
+    # search for whitespace
     for inx, char in enumerate(source):
         if char.isspace():
             result = inx
             break
 
     return result
 
@@ -70,15 +70,15 @@
     Extract and return the *substring* in *source* located between the delimiters *from_str* and *to_str*.
 
     :param source: the string to be inspected
     :param from_str: the initial delimiter
     :param to_str: the final delimiter
     :return: the extracted substring, or None if no substring was obtained
     """
-    # inicializa a variável de retorno
+    # initialize the return variable
     result: str | None = None
 
     pos1: int = source.find(from_str)
     if pos1 >= 0:
         pos1 += len(from_str)
         pos2: int = source.find(to_str, pos1)
         if pos2 >= pos1:
@@ -98,13 +98,13 @@
     """
     # declare the return variable
     result: str | None
 
     try:
         pos: int = list_origin.index(source)
         result = list_dest[pos]
-    except ValueError:
+    except (ValueError, IndexError):
         result = None
 
     return result
```

### Comparing `pypomes_core-0.8.4/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.8.5/src/pypomes_core/validation_msgs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Final
+from typing import Final, Literal
 
 __ERR_MSGS: Final[dict] = {
     101: {
         "en": "Error accessing the DB {} in {}: {}",
         "pt": "Erro na interação com o BD {} em {}: {}",
     },
     102: {
@@ -96,15 +96,15 @@
     _ERR_MSGS_EN[key] = value["en"]
 
 _ERR_MSGS_PT: dict = {}
 for key, value in __ERR_MSGS.items():
     _ERR_MSGS_PT[key] = value["pt"]
 
 
-def validate_add_msgs(msgs: dict, lang: str = "en") -> None:
+def validate_add_msgs(msgs: dict, lang: Literal["en", "pt"] = "en") -> None:
     """
     Add the messages in *msgs* to the standard validation messages list for language *lang".
 
     If applicable, this operation should be performed at the start of the application importing this module,
     before any attempt to read from *_ERR_MSGS_EN* or *_ERR_MSGS_PT*.
 
     :param msgs: list of messages to be added
@@ -113,15 +113,15 @@
     match lang:
         case "en":
             _ERR_MSGS_EN.update(msgs)
         case "pt":
             _ERR_MSGS_PT.update(msgs)
 
 
-def validate_set_msgs(msgs: dict, lang: str = "en") -> None:
+def validate_set_msgs(msgs: dict, lang: Literal["en", "pt"] = "en") -> None:
     """
     Set  the standard validation messages list for language *lang* to the messages in *msgs*.
 
     If applicable, this operation should be performed at the start of the application importing this module,
     before any attempt to read from *_ERR_MSGS_EN* or *_ERR_MSGS_PT*.
 
     :param msgs: list of messages to set the standard validation messages to
```

### Comparing `pypomes_core-0.8.4/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.8.5/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.4/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.8.5/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.4/LICENSE` & `pypomes_core-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.4/pyproject.toml` & `pypomes_core-0.8.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.8.4"
+version = "0.8.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.8.4/PKG-INFO` & `pypomes_core-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.8.4
+Version: 0.8.5
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

