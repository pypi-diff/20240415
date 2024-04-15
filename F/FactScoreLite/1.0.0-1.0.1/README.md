# Comparing `tmp/factscorelite-1.0.0.tar.gz` & `tmp/factscorelite-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factscorelite-1.0.0.tar", last modified: Sat Apr 13 23:42:24 2024, max compression
+gzip compressed data, was "factscorelite-1.0.1.tar", last modified: Mon Apr 15 02:57:11 2024, max compression
```

## Comparing `factscorelite-1.0.0.tar` & `factscorelite-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:42:24.926438 factscorelite-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:42:24.922438 factscorelite-1.0.0/FactScoreLite/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/atomic_facts.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:42:24.922438 factscorelite-1.0.0/FactScoreLite/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/data/demons.json
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/data/demons_generation_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/fact_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/factscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/openai_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/state_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:42:24.926438 factscorelite-1.0.0/FactScoreLite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-13 23:42:24.000000 factscorelite-1.0.0/FactScoreLite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-13 23:42:24.000000 factscorelite-1.0.0/FactScoreLite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 23:42:24.000000 factscorelite-1.0.0/FactScoreLite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 23:42:24.000000 factscorelite-1.0.0/FactScoreLite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 23:42:24.000000 factscorelite-1.0.0/FactScoreLite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-13 23:42:21.000000 factscorelite-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-13 23:42:24.926438 factscorelite-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-13 23:42:21.000000 factscorelite-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-13 23:42:24.926438 factscorelite-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 23:42:21.000000 factscorelite-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:42:24.926438 factscorelite-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 23:42:21.000000 factscorelite-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-13 23:42:21.000000 factscorelite-1.0.0/tests/test_atomic_facts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-13 23:42:21.000000 factscorelite-1.0.0/tests/test_fact_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-13 23:42:21.000000 factscorelite-1.0.0/tests/test_factscore.py
--rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-04-13 23:42:21.000000 factscorelite-1.0.0/tests/test_openai_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-13 23:42:21.000000 factscorelite-1.0.0/tests/test_state_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:57:11.243777 factscorelite-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:57:11.243777 factscorelite-1.0.1/FactScoreLite/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-15 02:57:03.000000 factscorelite-1.0.1/FactScoreLite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-04-15 02:57:03.000000 factscorelite-1.0.1/FactScoreLite/atomic_facts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-15 02:57:03.000000 factscorelite-1.0.1/FactScoreLite/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:57:11.243777 factscorelite-1.0.1/FactScoreLite/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-15 02:57:03.000000 factscorelite-1.0.1/FactScoreLite/data/demons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-15 02:57:03.000000 factscorelite-1.0.1/FactScoreLite/data/demons_generation_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-15 02:57:03.000000 factscorelite-1.0.1/FactScoreLite/fact_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-15 02:57:03.000000 factscorelite-1.0.1/FactScoreLite/factscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-15 02:57:03.000000 factscorelite-1.0.1/FactScoreLite/openai_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-15 02:57:03.000000 factscorelite-1.0.1/FactScoreLite/state_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:57:11.243777 factscorelite-1.0.1/FactScoreLite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-15 02:57:11.000000 factscorelite-1.0.1/FactScoreLite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-15 02:57:11.000000 factscorelite-1.0.1/FactScoreLite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:57:11.000000 factscorelite-1.0.1/FactScoreLite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 02:57:11.000000 factscorelite-1.0.1/FactScoreLite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 02:57:11.000000 factscorelite-1.0.1/FactScoreLite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-15 02:57:03.000000 factscorelite-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-15 02:57:11.243777 factscorelite-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-15 02:57:03.000000 factscorelite-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-15 02:57:11.247777 factscorelite-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:57:03.000000 factscorelite-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:57:11.243777 factscorelite-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 02:57:03.000000 factscorelite-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-15 02:57:03.000000 factscorelite-1.0.1/tests/test_atomic_facts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-15 02:57:03.000000 factscorelite-1.0.1/tests/test_fact_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-15 02:57:03.000000 factscorelite-1.0.1/tests/test_factscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-04-15 02:57:03.000000 factscorelite-1.0.1/tests/test_openai_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-15 02:57:03.000000 factscorelite-1.0.1/tests/test_state_handler.py
```

### Comparing `factscorelite-1.0.0/FactScoreLite/atomic_facts.py` & `factscorelite-1.0.1/FactScoreLite/atomic_facts.py`

 * *Files 13% similar despite different names*

```diff
@@ -182,23 +182,7 @@
                 results[-1] += " " + sent
                 combine_with_previous = False
             else:
                 assert not combine_with_previous
                 results.append(sent)
 
         return results
-
-
-if __name__ == "__main__":
-    generator = AtomicFactGenerator()
-    text = """
-        To winterize your battery and prevent damage:
-        
-        1. **For the Li-ion battery**:
-        - Avoid storing the vehicle in temperatures below -13°F (-25°C) for more than seven days to prevent the Li-ion battery from freezing.
-        - Move the vehicle to a warm location if the outside temperature is -13°F (-25°C) or below, as it may freeze and be unable to charge or power the vehicle.
-        
-        2. **For the 12-volt battery**:
-        - Ensure it is fully charged during extremely cold weather conditions to prevent the battery fluid from freezing and possibly causing damage to the battery.
-        """.strip()
-
-    print(generator.run(text))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `factscorelite-1.0.0/FactScoreLite/data/demons.json` & `factscorelite-1.0.1/FactScoreLite/data/demons.json`

 * *Files identical despite different names*

### Comparing `factscorelite-1.0.0/FactScoreLite/data/demons_generation_prompt.txt` & `factscorelite-1.0.1/FactScoreLite/data/demons_generation_prompt.txt`

 * *Files identical despite different names*

### Comparing `factscorelite-1.0.0/FactScoreLite/fact_scorer.py` & `factscorelite-1.0.1/FactScoreLite/fact_scorer.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             prompt += f"Context:\n{knowledge_source}"
 
             if not prompt[-1] in string.punctuation:
                 prompt += "."
 
             prompt += "\n\n"
 
-            prompt += f"Input:\n{atom} True or False?\nOutput:\n"
+            prompt += f"Input: {atom} True or False?\nOutput:\n"
 
             output = self.openai_agent.generate(prompt)
 
             generated_answer = output.lower()
             is_supported = None
 
             if "true" in generated_answer or "false" in generated_answer:
```

### Comparing `factscorelite-1.0.0/FactScoreLite/factscore.py` & `factscorelite-1.0.1/FactScoreLite/factscore.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from . import FactScorer, AtomicFactGenerator
 from .state_handler import StateHandler
 from . import configs
+from tqdm import tqdm
 
 
 class FactScore:
 
     def __init__(self, gamma: int = 10):
         self.atomic_fact_generator = AtomicFactGenerator()
         self.fact_scorer = FactScorer()
@@ -21,17 +22,19 @@
         Args:
             generations (list): A list of generations to extract facts from.
 
         Returns:
             list: A list of generation-facts pairs dictionaries.
         """
 
+        print("Extracting facts from generations...")
+
         generation_facts_pairs = self.facts_handler.load()
 
-        for generation in generations[len(generation_facts_pairs) :]:
+        for generation in tqdm(generations[len(generation_facts_pairs) :]):
             atomic_facts_of_generation = self.atomic_fact_generator.run(generation)
             atomic_facts_of_generation = [
                 fact
                 for sentence, atomic_facts in atomic_facts_of_generation
                 for fact in atomic_facts
             ]
             generation_facts_pairs.append(
@@ -44,14 +47,38 @@
 
         assert len(generation_facts_pairs) == len(
             generations
         ), "Number of generations and generation-facts pairs must match."
 
         return generation_facts_pairs
 
+    def calculate_score(self, decision: list) -> tuple:
+        """
+        Calculates the score of a generation based on whether its facts are supported by the knowledge source.
+
+        Args:
+            decision (list): A list containing dictionaries of {output, is_supported, fact} for each fact of a generation.
+
+        Returns:
+            tuple: A tuple containing the score and the original score (without applying gamma penalty).
+        """
+
+        score = np.mean([d["is_supported"] for d in decision])
+        init_score = score
+
+        if self.gamma:
+            penalty = (
+                1.0
+                if len(decision) >= self.gamma
+                else np.exp(1 - self.gamma / len(decision))
+            )
+            score = penalty * score
+
+        return score, init_score
+
     def get_decisions(
         self, generation_facts_pairs: list, knowledge_sources: list
     ) -> list:
         """
         Scores the facts related to each generation based on the according knowledge source.
         Uses FactScorer to score the facts and saves the results in a json file using the StateHandler.
 
@@ -62,49 +89,45 @@
         Returns:
             list:
                 A list of scores (scores after applying gamma penalty),
                 decisions (a dictionary containing output, is_supported, and the fact),
                 and initial scores (original score without applying gamma penalty).
         """
 
+        print("Generating decisions...")
+
         decisions = self.decisions_handler.load()
         scores = []
         init_scores = []
 
-        for entry in generation_facts_pairs[len(decisions) :]:
-            generation, facts = entry["generation"], entry["facts"]
-            score = None
+        for enrty in decisions:
+            score, init_score = self.calculate_score(enrty["decision"])
+            init_scores.append(init_score)
+            scores.append(score)
 
-            if facts:
-                decision = self.fact_scorer.get_score(facts, knowledge_sources)
-                score = np.mean([d["is_supported"] for d in decision])
-
-                if self.gamma:
-                    init_scores.append(score)
-                    penalty = (
-                        1.0
-                        if len(facts) > self.gamma
-                        else np.exp(1 - self.gamma / len(facts))
-                    )
-                    score = penalty * score
+        for entry in tqdm(generation_facts_pairs[len(decisions) :]):
+            generation, facts = entry["generation"], entry["facts"]
 
-                decisions.append({"generation": generation, "decision": decision})
-                self.decisions_handler.save(decisions)
+            decision = self.fact_scorer.get_score(facts, knowledge_sources)
+            score, init_score = self.calculate_score(decision)
 
+            init_scores.append(init_score)
             scores.append(score)
+            decisions.append({"generation": generation, "decision": decision})
+            self.decisions_handler.save(decisions)
 
             assert len(facts) == len(
                 decision
             ), "Number of facts and decisions for that generation should be the same."
 
         assert len(decisions) == len(
             generation_facts_pairs
         ), "Number of decisions and generation-facts pairs should be the same."
 
-        return scores, decisions, init_scores
+        return scores, init_scores
 
     def get_factscore(
         self,
         generations: list,
         knowledge_sources: list,
     ) -> tuple:
         """
@@ -120,10 +143,10 @@
         """
 
         assert len(generations) == len(
             knowledge_sources
         ), "`generations` and `knowledge_sources` should have the same length."
 
         facts = self.get_facts(generations)
-        scores, decisions, init_scores = self.get_decisions(facts, knowledge_sources)
+        scores, init_scores = self.get_decisions(facts, knowledge_sources)
 
         return np.mean(scores), np.mean(init_scores)
```

### Comparing `factscorelite-1.0.0/FactScoreLite/openai_agent.py` & `factscorelite-1.0.1/FactScoreLite/openai_agent.py`

 * *Files identical despite different names*

### Comparing `factscorelite-1.0.0/FactScoreLite.egg-info/PKG-INFO` & `factscorelite-1.0.1/FactScoreLite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FactScoreLite
-Version: 1.0.0
+Version: 1.0.1
 Summary: FactScore (Fine-grained atomic evaluation of factual precision in long form text generation) computing package.
 Home-page: https://github.com/armingh2000/FactScoreLite
 Author: armingh2000
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `factscorelite-1.0.0/FactScoreLite.egg-info/SOURCES.txt` & `factscorelite-1.0.1/FactScoreLite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `factscorelite-1.0.0/LICENSE` & `factscorelite-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `factscorelite-1.0.0/PKG-INFO` & `factscorelite-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FactScoreLite
-Version: 1.0.0
+Version: 1.0.1
 Summary: FactScore (Fine-grained atomic evaluation of factual precision in long form text generation) computing package.
 Home-page: https://github.com/armingh2000/FactScoreLite
 Author: armingh2000
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `factscorelite-1.0.0/README.md` & `factscorelite-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `factscorelite-1.0.0/setup.cfg` & `factscorelite-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FactScoreLite
-version = 1.0.0
+version = 1.0.1
 author = armingh2000
 author_email = 
 license = MIT
 description = FactScore (Fine-grained atomic evaluation of factual precision in long form text generation) computing package.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/armingh2000/FactScoreLite
```

### Comparing `factscorelite-1.0.0/tests/test_atomic_facts.py` & `factscorelite-1.0.1/tests/test_atomic_facts.py`

 * *Files identical despite different names*

### Comparing `factscorelite-1.0.0/tests/test_fact_scorer.py` & `factscorelite-1.0.1/tests/test_fact_scorer.py`

 * *Files identical despite different names*

### Comparing `factscorelite-1.0.0/tests/test_openai_agent.py` & `factscorelite-1.0.1/tests/test_openai_agent.py`

 * *Files identical despite different names*

### Comparing `factscorelite-1.0.0/tests/test_state_handler.py` & `factscorelite-1.0.1/tests/test_state_handler.py`

 * *Files identical despite different names*

