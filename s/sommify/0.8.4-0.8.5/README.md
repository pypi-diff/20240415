# Comparing `tmp/sommify-0.8.4.tar.gz` & `tmp/sommify-0.8.5.tar.gz`

## Comparing `sommify-0.8.4.tar` & `sommify-0.8.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sommify-0.8.4/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/__init__.py
--rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/regex.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/test.py
--rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/utils.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/countries/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/__init__.py
--rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/categories.py
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/constants.py
--rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/cuisine.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/embeddings.py
--rw-r--r--   0        0        0   356666 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_funnel.py
--rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredients.py
--rw-r--r--   0        0        0  5768681 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/mean_ing_embedding_per_tag.csv
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/meat.py
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/modifiers.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/vegetables.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/vulgar_fractions.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/cheeses.py
--rw-r--r--   0        0        0     8421 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/drinks.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/fruit.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/herbs.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/legumes.py
--rw-r--r--   0        0        0     7426 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/meats.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/nuts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/pasta.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/spices.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/vegetables.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/prompts/__init__.py
--rw-r--r--   0        0        0    47884 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/prompts/data/__init__.py
--rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/prompts/data/default.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/pygrape/__init__.py
--rw-r--r--   0        0        0   367143 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/pygrape/data.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/pynotesandhints/__init__.py
--rw-r--r--   0        0        0    63339 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/pynotesandhints/data.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/pyregion/__init__.py
--rw-r--r--   0        0        0    53240 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/pyregion/data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/recipes/__init__.py
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/recipes/elastic.py
--rw-r--r--   0        0        0    15852 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/recipes/reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/tests/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/tests/test_elastic.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/tests/test_prompts.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/tests/test_pygrape.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/tests/test_pyregion.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/tests/test_recipe_reader.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/tests/test_tag_reader.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 sommify-0.8.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sommify-0.8.4/LICENSE
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sommify-0.8.4/README.md
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 sommify-0.8.4/pyproject.toml
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 sommify-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sommify-0.8.5/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/__init__.py
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/regex.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/test.py
+-rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/utils.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/countries/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/__init__.py
+-rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/categories.py
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/constants.py
+-rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/cuisine.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/embeddings.py
+-rw-r--r--   0        0        0   356666 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_funnel.py
+-rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredients.py
+-rw-r--r--   0        0        0  5768681 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/mean_ing_embedding_per_tag.csv
+-rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/meat.py
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/modifiers.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/vegetables.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/vulgar_fractions.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/cheeses.py
+-rw-r--r--   0        0        0     8421 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/drinks.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/fruit.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/herbs.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/legumes.py
+-rw-r--r--   0        0        0     7426 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/meats.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/nuts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/pasta.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/spices.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/vegetables.py
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/prompts/__init__.py
+-rw-r--r--   0        0        0    47884 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/prompts/data/__init__.py
+-rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/prompts/data/default.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/pygrape/__init__.py
+-rw-r--r--   0        0        0   367143 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/pygrape/data.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/pynotesandhints/__init__.py
+-rw-r--r--   0        0        0    63339 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/pynotesandhints/data.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/pyregion/__init__.py
+-rw-r--r--   0        0        0    53240 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/pyregion/data.py
+-rw-r--r--   0        0        0    67688 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/recipes/__init__.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/recipes/elastic.py
+-rw-r--r--   0        0        0    15890 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/recipes/reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/tests/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/tests/test_elastic.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/tests/test_prompts.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/tests/test_pygrape.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/tests/test_pyregion.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/tests/test_recipe_reader.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/tests/test_tag_reader.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 sommify-0.8.5/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sommify-0.8.5/LICENSE
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sommify-0.8.5/README.md
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 sommify-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 sommify-0.8.5/PKG-INFO
```

### Comparing `sommify-0.8.4/sommify/regex.py` & `sommify-0.8.5/sommify/regex.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,16 @@
                     meat.type_portions[key] if key in meat.type_portions else 'all'
                 ] + meat.portions['general'])
             }))"""
         for key, values in meat.dictionary.items()
     ]
 )
 
+PORTION = one_of(meat.portions["all"])
+
 tests = [
     "175g/6oz piece smoked pancetta , rind removed",
     "1 inch x 2 inch large knob ginger",
     "1/4 cup celery , finely chopped",
     "3-4 lbs beef round steak",
     "1 1/2 head celery",
     "1kg 50g beef",
```

### Comparing `sommify-0.8.4/sommify/test.py` & `sommify-0.8.5/sommify/test.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/utils.py` & `sommify-0.8.5/sommify/utils.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/countries/__init__.py` & `sommify-0.8.5/sommify/countries/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/categories.py` & `sommify-0.8.5/sommify/data/categories.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/constants.py` & `sommify-0.8.5/sommify/data/constants.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/cuisine.py` & `sommify-0.8.5/sommify/data/cuisine.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/embeddings.py` & `sommify-0.8.5/sommify/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/ingredient_funnel.py` & `sommify-0.8.5/sommify/data/ingredient_funnel.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/ingredients.py` & `sommify-0.8.5/sommify/data/ingredients.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/mean_ing_embedding_per_tag.csv` & `sommify-0.8.5/sommify/data/mean_ing_embedding_per_tag.csv`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/meat.py` & `sommify-0.8.5/sommify/data/meat.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         r"balls?",
         r"carcass",
         r"medallions?",
         r"scampi",
     ],
     "pork": [
         r"trotters?",
-        r"shank",
+        r"shanks?",
         r"legs?",
         r"hogs?",
         r"loins?",
         r"bell(?:y|ies)",
         r"fillets?",
         r"shoulders?",
         r"necks?",
@@ -83,14 +83,15 @@
         r"rack",
         r"fatback",
         r"kidney",
         r"schnitzel",
         r"breast",
         r"brisket",
         r"cutlets?",
+        r"round",
     ],
     "beef": [
         r"shin",
         r"silver[- ]?side",
         r"kidneys?",
         r"top[- ]?side",
         r"short[- ]?rib",
@@ -104,47 +105,70 @@
         r"neck",
         r"bolo",
         r"wing[- ]?rib",
         r"chuck",
         r"brisket",
         r"round",
         r"meat",
+        r"roast",
         r"mince",
         r"oxtail",
         r"shoulder",
         r"heart",
         r"sirloin",
         r"jerky",
         r"tongue",
         r"ribs?",
         r"chunks?",
-        r"shank",
+        r"shanks?",
         r"medallions?",
         r"rump",
         r"chops?",
     ],
     "lamb": [
         r"neck",
         r"shoulder",
         r"chop",
         r"rack",
         r"loin",
         r"leg",
-        r"shank",
+        r"shanks?",
         r"meat",
         r"mince",
         r"kidney",
         r"rump",
         r"fillet",
         r"cutlet",
         r"belly",
         r"rib",
         r"breast",
+        r"shoulder joints?",
+        r"breast joints?",
+        r"rump joints?"
+        r"rib chops?",
+        r"leg chops?",
+        r"double blade chops?",
+        r"shoulder blade chops?",
+        r"shoulder chops?",
+        r"blade chops?",
+        r"chump chops?",
+        r"neck chops?",
+        r"neck fillets?",
+        r"meatballs?",
+        r"double cutlets?",
+        r"fore shanks?",
+        r"breast ribs?",
+    ],
+    "sausage": [
+        r"links?", 
+        r"rings?", 
+        r"casings?", 
+        r"meat", 
+        r"patty",
     ],
-    "sausage": [r"links?", r"rings?", r"casings?", r"meat", r"patty"],
     "general": [
         "mince",
         "meat",
         "chunk",
         "slice",
         "portion",
         "escalope",
@@ -167,22 +191,27 @@
     "sausage": [
         r"sausage(?:s|meat)?",
         r"chorizos?",
         r"kielbasas?",
         r"bratwursts?",
         r"longaniza",
         r"sai[- ]?ua",
+        r"sai kok",
         r"longganisas?",
-        r"lau[- ]?lau",
         r"chipolatas?",
         r"boudins?",
         r"bangers?",
         r"salpicao",
         r"salchichas?",
         r"salchichons?",
+        r"black[- ]?pudding",
+        r"white[- ]?pudding",
+        r"morcilla",
+        r"salami$", 
+        r"pepperoni$",
     ],
     "poultry": [r"chicken", "turkey", "rabbit", "hen"],
     "lamb": ["lamb", "mutton", "goat"],
     "game bird": [
         "pigeon",
         "pheasant",
         "quail",
@@ -301,14 +330,15 @@
         "serrano",
         "bresaola",
         "lomo",
     ],
     "beef": [
         "new york strip",
         "cow",
+        "entrec[oô]te",
         r"fill?et mignon",
         "loin",
         "tenderloin",
         "sirloin",
         r"beef[^s]",
         "wagyu",
         r"rib[ \-]eye",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sommify-0.8.4/sommify/data/modifiers.py` & `sommify-0.8.5/sommify/data/modifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,24 +25,27 @@
     "mild",
     "sharp",
     "firm",
     "soft",
     "aged",
     "thin",
     "thick",
+    r"thick[- ]cut",
+    r"center[- ]cut",
     "lean",
     "stoneground",
     r"\w+[- ]?style",
     r"(?:[0-9]+ [0-9]+/[0-9]+|[0-9]+)[- ]?inch(?:[ -]thick)?",
     r"\w+-sodium",
     r"\w+-fat",
     r"free[- ]range",
+    "french trimmed",
     "whole",
     "skin-on",
-    "hot",
+    # "hot",
     "cold",
     "warm",
     "boiling",
     r"\b(?<!\.)(?!0+(?:\.0+)?[ -]?%)(?:\d|[1-9]\d|100)(?:(?<!100)\.\d+)?[ -]?%",
     r"fresh(?:ly)?",
     r"[0-9]+[- ]bone",
     "quality",
```

### Comparing `sommify-0.8.4/sommify/data/vegetables.py` & `sommify-0.8.5/sommify/data/vegetables.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/ingredient_categories/__init__.py` & `sommify-0.8.5/sommify/data/ingredient_categories/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/ingredient_categories/drinks.py` & `sommify-0.8.5/sommify/data/ingredient_categories/drinks.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/ingredient_categories/fruit.py` & `sommify-0.8.5/sommify/data/ingredient_categories/fruit.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/ingredient_categories/herbs.py` & `sommify-0.8.5/sommify/data/ingredient_categories/herbs.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/ingredient_categories/meats.py` & `sommify-0.8.5/sommify/data/ingredient_categories/meats.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/ingredient_categories/nuts.py` & `sommify-0.8.5/sommify/data/ingredient_categories/nuts.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/ingredient_categories/spices.py` & `sommify-0.8.5/sommify/data/ingredient_categories/spices.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/data/ingredient_categories/vegetables.py` & `sommify-0.8.5/sommify/data/ingredient_categories/vegetables.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/prompts/__init__.py` & `sommify-0.8.5/sommify/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/prompts/data/__init__.py` & `sommify-0.8.5/sommify/prompts/data/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/prompts/data/default.py` & `sommify-0.8.5/sommify/prompts/data/default.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/pygrape/__init__.py` & `sommify-0.8.5/sommify/pygrape/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/pygrape/data.py` & `sommify-0.8.5/sommify/pygrape/data.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/pynotesandhints/__init__.py` & `sommify-0.8.5/sommify/pynotesandhints/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     def __len__(self) -> int:
         return len(self.notes_and_hints)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({len(self)})"
 
-    def get(self, **kwargs):
+    def get(self, **kwargs) -> NotesAndHint:
         return next(
             (
                 note
                 for note in self.notes_and_hints
                 if all(getattr(note, k) == v for k, v in kwargs.items())
             ),
             None,
```

### Comparing `sommify-0.8.4/sommify/pynotesandhints/data.py` & `sommify-0.8.5/sommify/pynotesandhints/data.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/pyregion/__init__.py` & `sommify-0.8.5/sommify/pyregion/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/pyregion/data.py` & `sommify-0.8.5/sommify/pyregion/data.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/recipes/elastic.py` & `sommify-0.8.5/sommify/recipes/elastic.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/recipes/reader.py` & `sommify-0.8.5/sommify/recipes/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,15 @@
 
     def read(
         self,
         title: str,
         phrases: list[str],
         steps: list[str] = list,
         ing_parsed: bool = False,
-        version: int = "v1",
+        version: str = "v1",
     ) -> object:
         parsed_phrases = [self.read_phrase(p) for p in phrases]
         parsed_phrases = self.merge_ingredients([p for p in parsed_phrases if p])
 
         if ing_parsed:
             ingredients = phrases
         else:
@@ -378,21 +378,21 @@
             "ingredients_": parsed_phrases,
             "title": title,
             "categories": categories,
             "models": _models,
             "values": values,
         }
 
-    def read_terms(self, input_term: str) -> object:
+    def read_terms(self, input_term: str, version: str = "v1") -> object:
         input_term = re.sub(r"\s+", " ", input_term)
         found_ings = self.extract_ingredients(input_term)
         title, ings, steps = elastic.search_by_query_term(
             self.es, input_term, found_ings
         )
-        return self.read(title, ings, steps, ing_parsed=True)
+        return self.read(title, ings, steps, ing_parsed=True, version=version)
 
 
 ING_EMBEDDING_LEN = 128
 TAG_EMBEDDING_LEN = 384
 
 
 class TagReader:
```

### Comparing `sommify-0.8.4/sommify/tests/test_elastic.py` & `sommify-0.8.5/sommify/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/tests/test_prompts.py` & `sommify-0.8.5/sommify/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/sommify/tests/test_recipe_reader.py` & `sommify-0.8.5/sommify/tests/test_recipe_reader.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/.gitignore` & `sommify-0.8.5/.gitignore`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/LICENSE` & `sommify-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sommify-0.8.4/pyproject.toml` & `sommify-0.8.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "sommify"
-version = "0.8.4"
+version = "0.8.5"
 authors = [
   { name="William Brach", email="william@sommify.ai" },
   { name="Tomas Bedej", email="tomas@sommify.ai" },
 ]
 description = "A package for recipe parsing"
 dependencies = [
   "inflect==7.0.0", 
@@ -41,15 +41,15 @@
     "F",  # pyflakes
     "I",  # isort
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
     "G",
     "SIM1",
     "PLE",
-    "N802", "N803", "N815", "N816","N806",
+    "N802", "N803", "N815", "N816", "N806",
     "ANN",
     "UP",  # pyupgrade,
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "C901",  # too complex
```

### Comparing `sommify-0.8.4/PKG-INFO` & `sommify-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sommify
-Version: 0.8.4
+Version: 0.8.5
 Summary: A package for recipe parsing
 Author-email: William Brach <william@sommify.ai>, Tomas Bedej <tomas@sommify.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

