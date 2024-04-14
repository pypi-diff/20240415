# Comparing `tmp/llm_structured_output-0.0.5.tar.gz` & `tmp/llm_structured_output-0.0.6.tar.gz`

## Comparing `llm_structured_output-0.0.5.tar` & `llm_structured_output-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/_/_build.sh
--rwxr-xr-x   0        0        0      467 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/_/_eval.sh
--rwxr-xr-x   0        0        0     1905 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/_/_mistral_schema.sh
--rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/_/_server.sh
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/_/_test_number_array.sh
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/_/_upload.sh
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/_/x.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/examples/json_schema_cli.py
--rw-r--r--   0        0        0    17802 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/examples/llm_schema.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/examples/requirements.txt
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/examples/server.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/llm_structured_output/__init__.py
--rw-r--r--   0        0        0    24610 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/llm_structured_output/acceptor.py
--rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/llm_structured_output/json_acceptor.py
--rw-r--r--   0        0        0    21187 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/llm_structured_output/json_schema_acceptor.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/llm_structured_output/util/__init__.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/llm_structured_output/util/bitmap.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/llm_structured_output/util/output.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/llm_structured_output/util/tokenization.py
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/llm_structured_output/util/tokentrie.py
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/tests/eval.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/src/tests/requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/LICENSE
--rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    14495 2020-02-02 00:00:00.000000 llm_structured_output-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/_build.sh
+-rwxr-xr-x   0        0        0      467 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/_eval.sh
+-rwxr-xr-x   0        0        0     1905 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/_mistral_schema.sh
+-rwxr-xr-x   0        0        0      853 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/_reluctance.sh
+-rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/_server.sh
+-rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/_test_number_array.sh
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/_upload.sh
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/_/x.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/examples/json_schema_cli.py
+-rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/examples/llm_schema.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/examples/reluctance.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/examples/requirements.txt
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/examples/server.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/__init__.py
+-rw-r--r--   0        0        0    24610 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/acceptor.py
+-rw-r--r--   0        0        0    14964 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/json_acceptor.py
+-rw-r--r--   0        0        0    21243 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/json_schema_acceptor.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/util/__init__.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/util/bitmap.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/util/output.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/util/tokenization.py
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/llm_structured_output/util/tokentrie.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/tests/eval.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/src/tests/requirements.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/LICENSE
+-rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    14495 2020-02-02 00:00:00.000000 llm_structured_output-0.0.6/PKG-INFO
```

### Comparing `llm_structured_output-0.0.5/_/_mistral_schema.sh` & `llm_structured_output-0.0.6/_/_mistral_schema.sh`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.5/_/x.py` & `llm_structured_output-0.0.6/_/x.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.5/src/examples/json_schema_cli.py` & `llm_structured_output-0.0.6/src/examples/json_schema_cli.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.5/src/examples/llm_schema.py` & `llm_structured_output-0.0.6/src/examples/llm_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # pylint: disable=missing-class-docstring,missing-function-docstring
 """
-Example of JSON schema decoding for Mixtral with MLX.
+Example of JSON schema decoding with MLX.
 """
 import argparse
 import json
 import time
+from math import inf
 from operator import itemgetter
 from typing import Iterable, Optional, Union
 
 import mlx.core as mx
 import mlx.nn as nn
 
 from mlx_lm.utils import load
 
 from llm_structured_output import JsonSchemaAcceptorDriver
-from llm_structured_output.util.bitmap import bias_logits, count_set_bits, enumerate_set_bits
+from llm_structured_output.util.bitmap import (
+    bias_logits,
+    count_set_bits,
+    enumerate_set_bits,
+)
 from llm_structured_output.util.output import info, bold, bolddim, debug
 from llm_structured_output.util.tokenization import HuggingfaceTokenizerHelper
 
 
 class RejectedCompletion(Exception):
     """
     It's rare, but sometimes we reach a state where it's not possible to
@@ -269,19 +274,19 @@
         model = self.model.model
         h = model.embed_tokens(inputs)
 
         mask = None
         T = h.shape[1]  # pylint: disable=invalid-name
         if T > 1:
             if cache is None:
-                N = 0  # pylint: disable=invalid-name
+                S = 0  # pylint: disable=invalid-name
             else:
-                N = cache[0][0].shape[2]  # pylint: disable=invalid-name
-            mask = nn.MultiHeadAttention.create_additive_causal_mask(N + T)
-            mask = mask.split([N])[1].astype(h.dtype)
+                S = cache[0][0].shape[2]  # pylint: disable=invalid-name
+            mask = nn.MultiHeadAttention.create_additive_causal_mask(S + T)
+            mask = mask.split([S])[1].astype(h.dtype)
 
         if cache is None:
             cache = [None] * len(model.layers)
 
         for e, layer in enumerate(model.layers):
             h, cache[e] = layer(h, mask, cache[e])
 
@@ -364,16 +369,20 @@
                 return
 
             start_time = time.time_ns()
 
         assert False
 
     def _debug_top_tokens(self, logits, count=10):
-        token_logits = sorted(enumerate(logits.tolist()), key=itemgetter(1), reverse=True)
-        top_tokens = [(self._decode([t]), p) for t, p in token_logits[:count]]
+        token_logits = sorted(
+            enumerate(logits.tolist()), key=itemgetter(1), reverse=True
+        )
+        top_tokens = [
+            (self._decode([t]), p) for t, p in token_logits[:count] if p != -inf
+        ]
         debug("TOP TOKENS:", top_tokens)
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="LLM inference script with schema-constrained sampling"
     )
@@ -397,15 +406,15 @@
     )
     parser.add_argument(
         "--temp",
         help="The sampling temperature.",
         type=float,
         default=0.0,
     )
-    parser.add_argument("--seed", type=int, default=0, help="The PRNG seed")
+    parser.add_argument("--seed", type=int, default=None, help="The PRNG seed")
     parser.add_argument(
         "--repeat-prompt",
         action=argparse.BooleanOptionalAction,
         help="Print prompt before start of generation",
     )
     parser.add_argument(
         "--schema",
```

### Comparing `llm_structured_output-0.0.5/src/examples/server.py` & `llm_structured_output-0.0.6/src/examples/server.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.5/src/llm_structured_output/acceptor.py` & `llm_structured_output-0.0.6/src/llm_structured_output/acceptor.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.5/src/llm_structured_output/json_acceptor.py` & `llm_structured_output-0.0.6/src/llm_structured_output/json_acceptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,36 +382,36 @@
 
     def __init__(self):
         super().__init__()
 
     def get_edges(self, state):
         return {
             0: [(TextAcceptor("{"), 1)],
-            1: [(WhitespaceAcceptor(), 2), (TextAcceptor("}"), "$")],
-            2: [(ObjectAcceptor.PropertyAcceptor(), 3)],
-            3: [(WhitespaceAcceptor(), 4)],
-            4: [
-                (SequenceAcceptor([TextAcceptor(","), WhitespaceAcceptor()]), 2),
-                (TextAcceptor("}"), "$"),
-            ],
+            1: [(self.EmptyTransition, 2), (self.EmptyTransition, 6)],
+            2: [(WhitespaceAcceptor(), 3)],
+            3: [(ObjectAcceptor.PropertyAcceptor(), 4)],
+            4: [(WhitespaceAcceptor(), 5)],
+            5: [(TextAcceptor(","), 2), (self.EmptyTransition, 7)],
+            6: [(WhitespaceAcceptor(), 7)],
+            7: [(TextAcceptor("}"), "$")],
         }[state]
 
     class Cursor(StateMachineAcceptor.Cursor):
         """
         Cursor for ObjectAcceptor
         """
 
         def __init__(self, acceptor):
             super().__init__(acceptor)
             self.value = {}
 
         def can_complete_transition(
             self, transition_value, target_state, is_end_state
         ) -> bool:
-            if self.current_state == 2:
+            if self.current_state == 3:
                 prop_name, prop_value = transition_value
                 self.value[prop_name] = prop_value
             return True
 
         def get_value(self):
             return self.value
```

### Comparing `llm_structured_output-0.0.5/src/llm_structured_output/json_schema_acceptor.py` & `llm_structured_output-0.0.6/src/llm_structured_output/json_schema_acceptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Acceptors for JSON schema validation or constraning LLM generation to JSON
 outputs complying with a JSON schema.
 """
+
 from __future__ import annotations
 
 import re
 from collections import defaultdict
 from typing import Iterable, Tuple
 
 from .acceptor import (
@@ -305,32 +306,26 @@
         self.schema = schema
         self.context = context
         self.properties = schema.get("properties")
         assert self.properties is not None
         super().__init__()
 
     def get_edges(self, state):
-        return {
-            0: lambda: [(TextAcceptor("{"), 1)],
-            1: lambda: [(WhitespaceAcceptor(), 2), (TextAcceptor("}"), "$")],
-            2: lambda: [
+        if state == 3:
+            return [
                 (
                     ObjectSchemaAcceptor.PropertyAcceptor(
                         prop_name, prop_schema, self.context
                     ),
-                    3,
+                    4,
                 )
                 for prop_name, prop_schema in self.properties.items()
-            ],
-            3: lambda: [(WhitespaceAcceptor(), 4)],
-            4: lambda: [
-                (SequenceAcceptor([TextAcceptor(","), WhitespaceAcceptor()]), 2),
-                (TextAcceptor("}"), "$"),
-            ],
-        }[state]()
+            ]
+        else:
+            return super().get_edges(state)
 
     def property_names(self):
         """
         Returns the names of the object's properties as defined in the schema
         """
         return self.schema.get("properties", {}).keys()
 
@@ -346,22 +341,24 @@
         """
 
         def __init__(self, acceptor):
             super().__init__(acceptor)
             self.acceptor = acceptor
 
         def can_attempt_transition(self, transition_acceptor, target_state) -> bool:
-            if self.current_state == 2 and target_state == 3:
+            if target_state == "$":
+                return all(
+                    prop_name in self.value
+                    for prop_name in self.acceptor.required_property_names()
+                )
+            if self.current_state == 3 and target_state == 4:
+                # Is a property already set?
                 return transition_acceptor.prop_name not in self.value
-            if self.current_state == 4:
-                if target_state == "$":
-                    return all(
-                        prop_name in self.value
-                        for prop_name in self.acceptor.required_property_names()
-                    )
+            if self.current_state == 5 and target_state == 2:
+                # Are all allowed properties already set?
                 return len(self.value.keys()) < len(self.acceptor.property_names())
             return True
 
     class PropertyAcceptor(ObjectAcceptor.PropertyAcceptor):
         """
         Acceptor for an object property according to the schema
         """
@@ -591,14 +588,19 @@
     def __init__(
         self,
         schema: dict,
         vocabulary: Iterable[Tuple[int, str]],
         eos_id: int,
         is_encapsulated_json: bool = False,
     ):
+        # Make sure the eos token is removed.
+        # Ideally, the caller should not pass any special tokens (bos, eos, unk, pad, ...)
+        vocabulary = [
+            (token, fragment) for token, fragment in vocabulary if token != eos_id
+        ]
         self.trie = TokenAcceptor.prepare_vocabulary(vocabulary)
         prepare_json_acceptor_tries(self.trie)
         self.eos_id = eos_id
         if is_encapsulated_json:
             self.acceptor = EncapsulatedJsonSchemaAcceptor(schema)
         else:
             self.acceptor = JsonSchemaAcceptor(schema)
```

### Comparing `llm_structured_output-0.0.5/src/llm_structured_output/util/bitmap.py` & `llm_structured_output-0.0.6/src/llm_structured_output/util/bitmap.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,40 +12,63 @@
     """
     # FUTURE: self.ids.bit_count() available from Python 3.10 is said to be 6x faster
     return bin(bitmap).count("1")
 
 
 def highest_bit_set(bitmap: int) -> int:
     """
-    Return the highest bit set in the bitmap.
+    Return the index of the highest bit set in the bitmap.
     """
     return bitmap.bit_length() - 1
 
 
+def bitmap_complement(bitmap: int, set_size: int = None) -> int:
+    """
+    Negate the bits in the bitmap.
+    Since the bitmap is encoded as a Python int, it can be of arbitrary length.
+    I.e. we don't know how many zeros are above the top set bit. The set_size
+    parameter can be passed to indicate the number of bits in the bitmap (which
+    is akin to the number of members in the set it represents). If unspecified,
+    the top set bit in the bitmap is used as its set size. 
+    """
+    if not set_size:
+        set_size = bitmap.bit_length()
+    return (1 << set_size) - 1 - bitmap
+
+
 def enumerate_set_bits(bitmap: int) -> Iterable[int]:
     """
     Generator that yields the indices of the set bits in the bitmap.
     Note that it does so from highest to lowest.
     """
     while bitmap:
         highest_bit = highest_bit_set(bitmap)
         yield highest_bit
         bitmap -= 1 << highest_bit
 
 
 def bias_logits(np, logits, accepted_token_bitmap):
     """
     Apply a -inf bias to tokens that will not be accepted.
+    Rather than import here, the np parameters is numpy or a compatible library
+    import, such as mlx.core.
     """
-    highest_token = highest_bit_set(accepted_token_bitmap)
-    match_count = count_set_bits(accepted_token_bitmap)
+    vocab_size = logits.shape[0]
+    highest_token_accepted = highest_bit_set(accepted_token_bitmap)
+    accepted_token_count = count_set_bits(accepted_token_bitmap)
     # Check whether there's more tokens to be rejected or to be allowed, then do what's less work.
-    if match_count <= highest_token / 2:
+    if accepted_token_count <= highest_token_accepted / 2:
+        bias = np.full(vocab_size, -inf)
         indices = np.array([*enumerate_set_bits(accepted_token_bitmap)])
-        array = np.full(logits.shape, -inf)
-        array[indices] = 0
+        bias[indices] = 0
     else:
-        rejected_token_bitmap = (1 << (highest_token + 1)) - 1 - accepted_token_bitmap
+        bias = np.concatenate(
+            [
+                np.full(highest_token_accepted + 1, 0),
+                # All tokens above the highest accepted token are rejected.
+                np.full(vocab_size - highest_token_accepted - 1, -inf),
+            ]
+        )
+        rejected_token_bitmap = bitmap_complement(accepted_token_bitmap)
         indices = np.array([*enumerate_set_bits(rejected_token_bitmap)])
-        array = np.full(logits.shape, 0)
-        array[indices] = -inf
-    return np.add(logits, array)
+        bias[indices] = -inf
+    return np.add(logits, bias)
```

### Comparing `llm_structured_output-0.0.5/src/llm_structured_output/util/output.py` & `llm_structured_output-0.0.6/src/llm_structured_output/util/output.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pylint: disable=missing-function-docstring
 """
 Terminal colored output
 """
 
+
 def info(*args, **kwargs):
     print("\033[34mℹ ", end="")
     print(*args, **kwargs)
     print("\033[0m", end="")
 
 
 def warning(*args, **kwargs):
@@ -51,7 +52,23 @@
     print("\033[0m", end="")
 
 
 def inverse(*args, **kwargs):
     print("\033[7m", end="")
     print(*args, **kwargs)
     print("\033[0m", end="")
+
+
+def setfg(r: float, g: float, b: float):
+    """Each of r,g,b must be between 0 and 1"""
+    color = 16 + 36 * round(5 * r) + 6 * round(5 * g) + round(5 * b)
+    print(f"\033[38;5;{color}m", end="")
+
+
+def setbg(r: float, g: float, b: float):
+    """Each of r,g,b must be between 0 and 1"""
+    color = 16 + 36 * round(5 * r) + 6 * round(5 * g) + round(5 * b)
+    print(f"\033[48;5;{color}m", end="")
+
+
+def clear():
+    print("\033[0m", end="")
```

### Comparing `llm_structured_output-0.0.5/src/llm_structured_output/util/tokenization.py` & `llm_structured_output-0.0.6/src/llm_structured_output/util/tokenization.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.5/src/llm_structured_output/util/tokentrie.py` & `llm_structured_output-0.0.6/src/llm_structured_output/util/tokentrie.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.5/src/tests/eval.py` & `llm_structured_output-0.0.6/src/tests/eval.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from deepdiff import DeepDiff
 
 from examples.llm_schema import Model
 from llm_structured_output.util.output import info, bold, inverse, debug
 
 
-def run_eval_case(model, case, header):
+def run_eval_case(model, case, header, temp=None, seed=None, preemptive_batch_size=0):
     messages = case["prompt"]
     gold_completion = json.loads(case["completion"].partition("<functioncall>")[2])
     tools = json.loads(case["tools"])
 
     schema = {
         "anyOf": [
             {
@@ -47,15 +47,17 @@
     completion_tokens = 0
     completion_time = 0
 
     for result in model.completion(
         messages,
         schema=schema,
         max_tokens=4000,
-        temp=0,
+        temp=temp,
+        seed=seed,
+        preemptive_batch_size=preemptive_batch_size,
     ):
         if result["op"] == "evaluatedPrompt":
             prompt_tokens += result["token_count"]
             prompt_time = result["time_ms"]
         elif result["op"] == "generatedTokens":
             completion_tokens += result["token_count"]
             completion_time += result["time_ms"]
@@ -106,14 +108,27 @@
     )
     parser.add_argument(
         "--count",
         type=int,
         default=None,
         help="Limit the number of cases to run",
     )
+    parser.add_argument(
+        "--temp",
+        help="The sampling temperature.",
+        type=float,
+        default=0.0,
+    )
+    parser.add_argument("--seed", type=int, default=0, help="The PRNG seed")
+    parser.add_argument(
+        "--preemptive",
+        type=int,
+        default=0,
+        help="If greater than zero, the maximum size of the batch for pre-emptive decoding",
+    )
     args = parser.parse_args()
 
     info("Loading model...")
     model = Model()
     model.load(args.model_path)
 
     with open(args.dataset_path, encoding="utf-8") as dataset:
@@ -121,16 +136,23 @@
         pass_count = 0
         fail_count = 0
         t0 = time.time_ns()
         if args.count:
             end_index = args.skip + args.count
         else:
             end_index = len(cases)
-        for i, case in enumerate(cases[args.skip:end_index]):
-            if run_eval_case(model, case, f"[{i+args.skip}]"):
+        for i, case in enumerate(cases[args.skip : end_index]):
+            if run_eval_case(
+                model,
+                case,
+                f"[{i+args.skip}]",
+                temp=args.temp,
+                seed=args.seed,
+                preemptive_batch_size=args.preemptive,
+            ):
                 pass_count += 1
             else:
                 fail_count += 1
         average_time = (time.time_ns() - t0) / 1e9 / (pass_count + fail_count)
         info(f"Totals: {pass_count=} {fail_count=} {average_time=:.02}s")
```

### Comparing `llm_structured_output-0.0.5/LICENSE` & `llm_structured_output-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.5/README.md` & `llm_structured_output-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.5/pyproject.toml` & `llm_structured_output-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "llm_structured_output"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Oscar D.P. Triscon", email="github@triscon.com" },
 ]
 description = "Constrain LLM generation to structured output, such as function calling a.k.a. tool use"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `llm_structured_output-0.0.5/PKG-INFO` & `llm_structured_output-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: llm_structured_output
-Version: 0.0.5
+Version: 0.0.6
 Summary: Constrain LLM generation to structured output, such as function calling a.k.a. tool use
 Project-URL: Homepage, https://github.com/otriscon/llm-structured-output
 Project-URL: Issues, https://github.com/otriscon/llm-structured-output/issues
 Author-email: "Oscar D.P. Triscon" <github@triscon.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

