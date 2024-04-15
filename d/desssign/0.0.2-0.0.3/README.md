# Comparing `tmp/desssign-0.0.2.tar.gz` & `tmp/desssign-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desssign-0.0.2.tar", max compression
+gzip compressed data, was "desssign-0.0.3.tar", max compression
```

## Comparing `desssign-0.0.2.tar` & `desssign-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,37 @@
--rw-r--r--   0        0        0     1070 2024-03-06 10:39:18.677196 desssign-0.0.2/LICENSE
--rw-r--r--   0        0        0     2765 2024-03-06 10:39:18.677196 desssign-0.0.2/README.md
--rw-r--r--   0        0        0     4214 2024-03-06 10:39:28.393288 desssign-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       16 2024-03-06 10:39:18.677196 desssign-0.0.2/src/desssign/__init__.py
--rw-r--r--   0        0        0      207 2024-03-06 10:39:18.677196 desssign-0.0.2/src/desssign/__main__.py
--rw-r--r--   0        0        0        0 2024-03-06 10:39:18.677196 desssign-0.0.2/src/desssign/loads/__init__.py
--rw-r--r--   0        0        0     4510 2024-03-06 10:39:18.677196 desssign-0.0.2/src/desssign/loads/combination_group.py
--rw-r--r--   0        0        0     2860 2024-03-06 10:39:18.677196 desssign-0.0.2/src/desssign/loads/enums.py
--rw-r--r--   0        0        0      980 2024-03-06 10:39:18.677196 desssign-0.0.2/src/desssign/loads/load_case.py
--rw-r--r--   0        0        0      503 2024-03-06 10:39:18.677196 desssign-0.0.2/src/desssign/loads/load_combination.py
--rw-r--r--   0        0        0        0 2024-03-06 10:39:18.677196 desssign-0.0.2/src/desssign/loads/load_combination_generator/__init__.py
--rw-r--r--   0        0        0     2046 2024-03-06 10:39:18.677196 desssign-0.0.2/src/desssign/loads/load_combination_generator/constants.py
--rw-r--r--   0        0        0     7794 2024-03-06 10:39:18.677196 desssign-0.0.2/src/desssign/loads/load_combination_generator/generate_combinations.py
--rw-r--r--   0        0        0     2301 2024-03-06 10:39:18.677196 desssign-0.0.2/src/desssign/loads/load_group.py
--rw-r--r--   0        0        0        0 2024-03-06 10:39:18.677196 desssign-0.0.2/src/desssign/py.typed
--rw-r--r--   0        0        0      960 2024-03-06 10:39:18.677196 desssign-0.0.2/src/desssign/utils.py
--rw-r--r--   0        0        0        0 2024-03-06 10:39:18.677196 desssign-0.0.2/src/desssign/wood/__init__.py
--rw-r--r--   0        0        0     9511 2024-03-06 10:39:18.681196 desssign-0.0.2/src/desssign/wood/strength_classes.py
--rw-r--r--   0        0        0     3733 1970-01-01 00:00:00.000000 desssign-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-15 18:34:16.168453 desssign-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2765 2024-04-15 18:34:16.168453 desssign-0.0.3/README.md
+-rw-r--r--   0        0        0     4390 2024-04-15 18:34:26.348602 desssign-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       16 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/__init__.py
+-rw-r--r--   0        0        0      207 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/__main__.py
+-rw-r--r--   0        0        0       53 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/__init__.py
+-rw-r--r--   0        0        0     4251 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/enums.py
+-rw-r--r--   0        0        0     1544 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/load_case.py
+-rw-r--r--   0        0        0     5178 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/load_case_combination.py
+-rw-r--r--   0        0        0     2536 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/load_case_group.py
+-rw-r--r--   0        0        0       60 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/load_combination_generator/__init__.py
+-rw-r--r--   0        0        0     7915 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/load_combination_generator/combination_generator.py
+-rw-r--r--   0        0        0     1974 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/load_combination_generator/constants.py
+-rw-r--r--   0        0        0    11096 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/load_combination_generator/generate_combinations.py
+-rw-r--r--   0        0        0       29 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/snow/__init__.py
+-rw-r--r--   0        0        0      424 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/snow/constants.py
+-rw-r--r--   0        0        0      464 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/snow/enums.py
+-rw-r--r--   0        0        0     2295 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/snow/snow_load.py
+-rw-r--r--   0        0        0       29 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/wind/__init__.py
+-rw-r--r--   0        0        0     1036 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/wind/constants.py
+-rw-r--r--   0        0        0      863 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/wind/enums.py
+-rw-r--r--   0        0        0    17926 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/wind/external_pressure_coefficients.py
+-rw-r--r--   0        0        0    17663 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/wind/roofs.py
+-rw-r--r--   0        0        0     4753 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/loads/wind/wind_load.py
+-rw-r--r--   0        0        0        0 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/py.typed
+-rw-r--r--   0        0        0      973 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/utils.py
+-rw-r--r--   0        0        0       30 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/wood/__init__.py
+-rw-r--r--   0        0        0     4149 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/wood/constants.py
+-rw-r--r--   0        0        0    13194 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/wood/design_checks/design_check.py
+-rw-r--r--   0        0        0    12342 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/wood/design_checks/member_1d_checks.py
+-rw-r--r--   0        0        0     1866 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/wood/enums.py
+-rw-r--r--   0        0        0     7364 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/wood/models.py
+-rw-r--r--   0        0        0    10012 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/wood/strength_classes.py
+-rw-r--r--   0        0        0     3620 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/wood/wood_material.py
+-rw-r--r--   0        0        0     6398 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/wood/wood_member.py
+-rw-r--r--   0        0        0     3500 2024-04-15 18:34:16.172453 desssign-0.0.3/src/desssign/wood/wood_section.py
+-rw-r--r--   0        0        0     3733 1970-01-01 00:00:00.000000 desssign-0.0.3/PKG-INFO
```

### Comparing `desssign-0.0.2/LICENSE` & `desssign-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `desssign-0.0.2/README.md` & `desssign-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `desssign-0.0.2/pyproject.toml` & `desssign-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "desssign"
-version = "0.0.2"
+version = "0.0.3"
 description = "desssign"
 authors = ["Daniel Beranek <daniel.beraanek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DanBeranek/desssign"
 repository = "https://github.com/DanBeranek/desssign"
 documentation = "https://DanBeranek.github.io/desssign"
@@ -14,15 +14,15 @@
 Changelog = "https://github.com/DanBeranek/desssign/releases"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = ">=8.0.1"
 numpy = "^1.26.4"
 aenum = "^3.1.15"
-framesss = "^0.0.2"
+framesss = "^0.0.3"
 
 [tool.poetry.group.dev.dependencies]
 pygments = ">=2.10.0"
 black = { extras = ["jupyter"], version = ">=23.1.0" }
 coverage = { extras = ["toml"], version = ">=6.2" }
 darglint = ">=1.8.1"
 furo = ">=2021.11.12"
@@ -133,12 +133,15 @@
     "ANN205",  # type annotations don't add value for test functions
     "ANN206",  # type annotations don't add value for test functions
     "D100",    # docstrings are overkill for test functions
     "D101",
     "D102",
     "D103",
     "S101",    # asserts are encouraged in pytest
+    "E741",    # ignore ambigious variable name
 ]
+"**/wind/enums.py" = ["E741"]  # ignore ambigious variable name
+"**/snow/enums.py" = ["E741"]  # ignore ambigious variable name
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `desssign-0.0.2/src/desssign/loads/combination_group.py` & `desssign-0.0.3/src/desssign/loads/load_case_combination.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,121 @@
 from __future__ import annotations
 
-from itertools import product
-from typing import TYPE_CHECKING
+from typing import cast
 
+from framesss.pre.cases import LoadCase
+from framesss.pre.cases import LoadCaseCombination
+
+from desssign.loads.enums import LOAD_DURATION_MAPPING
 from desssign.loads.enums import LimitState
-from desssign.loads.enums import LoadType
+from desssign.loads.enums import LoadDurationClass
 from desssign.loads.enums import SLSCombination
+from desssign.loads.enums import ULSAlternativeCombination
 from desssign.loads.enums import ULSCombination
+from desssign.loads.load_case import DesignLoadCase
 from desssign.loads.load_combination_generator.generate_combinations import (
     generate_combination,
 )
-from desssign.utils import flatten_list
 
-if TYPE_CHECKING:
-    from desssign.loads.load_combination import DesignLoadCombination
-    from desssign.loads.load_group import LoadGroup
 
+class DesignLoadCaseCombination(LoadCaseCombination):
+    """
+    Represent a combination of load cases in the design process.
+
+    :param label: The label of the load case combination.
+    :param limit_state: The limit state of the combination group. Either 'ULS' or 'SLS'.
+    :param combination_type: The type of the combination group. For ULS: basic, alternative or accidental,
+                             for SLS: characteristic, frequent or quasi-permanent.
+    :param permanent_cases: A list of permanent load cases.
+    :param leading_variable_case: The leading variable load case.
+    :param other_variable_cases: A list of other variable load cases.
+    :param alternative_combination: Specifier for the used equation, only required for ULS alternative combinations.
+                                    Either '6.10a' or '6.10b'.
+    :ivar combination_key: The key of the combination.
+    """
 
-class CombinationGroup:
     def __init__(
         self,
+        label: str,
         limit_state: str | LimitState,
         combination_type: str | SLSCombination | ULSCombination,
+        permanent_cases: list[DesignLoadCase],
+        leading_variable_case: DesignLoadCase | None,
+        other_variable_cases: list[DesignLoadCase],
+        alternative_combination: str | ULSAlternativeCombination | None = None,
     ) -> None:
-        """Init the CombinationGroup class."""
+        """Initialize the DesignLoadCaseCombination class."""
         self.limit_state = LimitState(limit_state)
 
         if self.limit_state == LimitState.ULS:
             self.combination_type = ULSCombination(combination_type)
         elif self.limit_state == LimitState.SLS:
             self.combination_type = SLSCombination(combination_type)
         else:
-            raise AttributeError(
+            raise ValueError(
                 f"Can't set combination type: '{combination_type}' to limit state: '{limit_state}'."
             )
 
-        self.combinations: list[DesignLoadCombination] = []
-
-    def generate_combinations(self, *args: list[LoadGroup]) -> None:
-        # get all possible combinations
-        all_iterables = []
-        for load_groups in args:
-            all_iterables.append(
-                [load_group.combinations for load_group in load_groups]
-            )
-
-        combinations = []
-        for iterables in all_iterables:
-            combinations.extend(
-                [flatten_list(combination) for combination in product(*iterables)]
-            )
-
-        # get all possible unique combinations
-        unique_combinations = []
-        for combination in combinations:
-            if combination not in unique_combinations:
-                unique_combinations.append(combination)
-
-        c = 0
-        for unique_combination in unique_combinations:
-            permanent_cases = [
-                case
-                for case in unique_combination
-                if case.load_type == LoadType.PERMANENT
-            ]
-            variable_cases = [
-                case
-                for case in unique_combination
-                if case.load_type == LoadType.VARIABLE
-            ]
-
-            if variable_cases:
-                for i, leading_variable_case in enumerate(variable_cases):
-                    # loop through every possible combination of leading + other variable for this unique combination
-                    other_variable_cases = variable_cases[:i] + variable_cases[i + 1:]
-
-                    self.combinations.extend(
-                        generate_combination(
-                            c,
-                            permanent_cases,
-                            leading_variable_case,
-                            other_variable_cases,
-                            self.combination_type,
-                        )
-                    )
-
-                    c += 1
-            else:  # in case there is only permanent cases
-                self.combinations.extend(
-                    generate_combination(
-                        c, permanent_cases, None, [], self.combination_type
-                    )
+        if combination_type == ULSCombination.ALTERNATIVE:
+            if alternative_combination is None:
+                raise ValueError(
+                    "Alternative combination requires an 'alternative_combination'."
                 )
-                c += 1
 
+        self.alternative_combination = (
+            ULSAlternativeCombination(alternative_combination)
+            if alternative_combination
+            else None
+        )
+
+        self.permanent_cases = permanent_cases
+        self.leading_variable_case = leading_variable_case
+        self.other_variable_cases = other_variable_cases
+
+        load_cases, self.combination_key = generate_combination(
+            permanent_cases=self.permanent_cases,
+            leading_variable_case=self.leading_variable_case,
+            other_variable_cases=self.other_variable_cases,
+            combination=self.combination_type,
+            alternative_combination=self.alternative_combination,
+        )
+
+        super().__init__(label, cast(dict[LoadCase, float], load_cases))
+
+    def _get_combination(self) -> tuple[dict[DesignLoadCase, float], str]:
+        """Return the load cases combination and the combination key."""
+        return generate_combination(
+            permanent_cases=self.permanent_cases,
+            leading_variable_case=self.leading_variable_case,
+            other_variable_cases=self.other_variable_cases,
+            combination=self.combination_type,
+            alternative_combination=self.alternative_combination,
+        )
+
+    @property
+    def load_duration_class(self) -> LoadDurationClass:
+        """
+        Return the load duration class of the combination.
+
+        EN 1995-1-1, 3.1.3(2):
+            If a load combination consists of actions belonging to different load-duration classes a value
+            of `k_mod` should be chosen which corresponds to the action with the shortest duration, e.g. for a
+            combination of dead load and a short-term load, a value of k_mod corresponding to the short-term
+            load should be used.
+        """
+        # Get the minimum value of all duration classes
+        min_duration_value = min(
+            [
+                LOAD_DURATION_MAPPING[cast(DesignLoadCase, case).load_duration_class]
+                for case in self.load_cases
+            ]
+        )
 
-if __name__ == "__main__":
-    from desssign.loads.load_case import DesignLoadCase
-    from desssign.loads.load_group import LoadGroup
-
-    G1 = DesignLoadCase("G1", "permanent")
-    G2 = DesignLoadCase("G2", "permanent")
-    LG1 = LoadGroup([G1, G2], "together")
-
-    Q1 = DesignLoadCase("Q1", "variable", "category a")
-    Q2 = DesignLoadCase("Q2", "variable", "category b")
-    LG2 = LoadGroup([Q1, Q2], "standard")
-
-    S1 = DesignLoadCase("S1", "variable", "snow < 1000 m")
-    S2 = DesignLoadCase("S2", "variable", "snow < 1000 m")
-    S3 = DesignLoadCase("S3", "variable", "snow < 1000 m")
-    LG3 = LoadGroup([S1, S2, S3], "exclusive")
-
-    W1 = DesignLoadCase("W1", "variable", "wind")
-    W2 = DesignLoadCase("W2", "variable", "wind")
-    W3 = DesignLoadCase("W3", "variable", "wind")
-    W4 = DesignLoadCase("W4", "variable", "wind")
-    LG4 = LoadGroup([W1, W2, W3, W4], "exclusive")
-
-    ULS = CombinationGroup("ULS", "basic")
-
-    ULS.generate_combinations([LG1, LG2], [LG1, LG3, LG4])
-
-    for comb in ULS.combinations:
-        print(comb.combination_key)
-
-    print("")
+        # Find the LoadDurationClass corresponding to the minimum value
+        for duration_class, value in LOAD_DURATION_MAPPING.items():
+            if value == min_duration_value:
+                return LoadDurationClass(duration_class)
+
+        # If no matching LoadDurationClass is found, raise an exception
+        raise ValueError(
+            f"Can't find the load duration class with value: '̈́{min_duration_value}'."
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `desssign-0.0.2/src/desssign/loads/enums.py` & `desssign-0.0.3/src/desssign/loads/enums.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from framesss.enums import CaseInsensitiveStrEnum
 
 
 class LoadBehavior(CaseInsensitiveStrEnum):
+    """Enumeration of possible behavior of action."""
+
     UNFAVOURABLE = "unfavourable"
     FAVOURABLE = "favourable"
 
 
 class LoadType(CaseInsensitiveStrEnum):
     """Enumeration of possible type of action."""
 
@@ -50,14 +52,26 @@
     """
 
     BASIC = "basic"
     ALTERNATIVE = "alternative"
     ACCIDENTAL = "accidental"
 
 
+class ULSAlternativeCombination(CaseInsensitiveStrEnum):
+    """
+    Enumeration of ULS alternative combination types.
+
+    :cvar REDUCED_PERMANENT: Combination with reduced permanent load cases.
+    :cvar REDUCED_VARIABLE: Combination with reduced leading variable load case.
+    """
+
+    REDUCED_VARIABLE = "6.10a"
+    REDUCED_PERMANENT = "6.10b"
+
+
 class SLSCombination(CaseInsensitiveStrEnum):
     """
     Enumeration of serviceability limit state combinations according to EN 1990.
 
     :cvar CHARACTERISTIC: Combination according to equations 6.14 of EN 1990.
     :cvar FREQUENT: Combination according to equation 6.15 of EN 1990.
     :cvar QUASIPERMANENT: Combination according to equation 6.16 of EN 1990.
@@ -67,22 +81,22 @@
     FREQUENT = "frequent"
     QUASIPERMANENT = "quasipermanent"
 
 
 class VariableCategory(CaseInsensitiveStrEnum):
     """Enumeration of possible variable loads."""
 
-    CATEGORY_A = "category a"
-    CATEGORY_B = "category b"
-    CATEGORY_C = "category c"
-    CATEGORY_D = "category d"
-    CATEGORY_E = "category e"
-    CATEGORY_F = "category f"
-    CATEGORY_G = "category g"
-    CATEGORY_H = "category h"
+    A = "a"
+    B = "b"
+    C = "c"
+    D = "d"
+    E = "e"
+    F = "f"
+    G = "g"
+    H = "h"
     SNOW_ABOVE_1000_M = "snow > 1000 m"
     SNOW_BELLOW_1000_M = "snow < 1000 m"
     WIND = "wind"
     TEMPERATURE = "temperature"
 
 
 class LoadCaseRelation(CaseInsensitiveStrEnum):
@@ -93,7 +107,40 @@
     :cvar STANDARD: Load cases from the same load group may (or may not) act together.
     :cvar TOGETHER: Load cases from the same load group always act together.
     """
 
     EXCLUSIVE = "exclusive"
     STANDARD = "standard"
     TOGETHER = "together"
+
+
+class LoadDurationClass(CaseInsensitiveStrEnum):
+    """
+    Enum for load duration classes.
+
+    EN 1995-1-1, 2.3.1.2 Load-duration classes.
+
+    The load-duration classes are characterised by the effect of a constant load acting for a
+    certain period of time in the life of the structure. For a variable action the appropriate class shall
+    be determined on the basis of an estimate of the typical variation of the load with time.
+
+    :cvar PERMANENT: more than 10 years, e.g. self-weight
+    :cvar LONG_TERM: 6 months - 10 years, e.g. storage
+    :cvar MEDIUM_TERM: 1 week - 6 months, e.g. imposed floor load, snow
+    :cvar SHORT_TERM: less than 1 week, e.g. snow, wind
+    :cvar INSTANTANEOUS: instantaneous, e.g. wind, accidental load
+    """
+
+    PERMANENT = "permanent"
+    LONG_TERM = "long-term"
+    MEDIUM_TERM = "medium-term"
+    SHORT_TERM = "short-term"
+    INSTANTANEOUS = "instantaneous"
+
+
+LOAD_DURATION_MAPPING = {
+    LoadDurationClass.INSTANTANEOUS: 1,
+    LoadDurationClass.SHORT_TERM: 2,
+    LoadDurationClass.MEDIUM_TERM: 3,
+    LoadDurationClass.LONG_TERM: 4,
+    LoadDurationClass.PERMANENT: 5,
+}
```

### Comparing `desssign-0.0.2/src/desssign/loads/load_combination_generator/constants.py` & `desssign-0.0.3/src/desssign/loads/load_combination_generator/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from desssign.loads.enums import LoadBehavior
 from desssign.loads.enums import LoadType
 from desssign.loads.enums import VariableCategory
 
 PSI_FACTORS = {
-    VariableCategory.CATEGORY_A: {
+    VariableCategory.A: {
         "psi_0": 0.7,
         "psi_1": 0.5,
         "psi_2": 0.3,
     },
-    VariableCategory.CATEGORY_B: {
+    VariableCategory.B: {
         "psi_0": 0.7,
         "psi_1": 0.5,
         "psi_2": 0.3,
     },
-    VariableCategory.CATEGORY_C: {
+    VariableCategory.C: {
         "psi_0": 0.7,
         "psi_1": 0.7,
         "psi_2": 0.6,
     },
-    VariableCategory.CATEGORY_D: {
+    VariableCategory.D: {
         "psi_0": 0.7,
         "psi_1": 0.7,
         "psi_2": 0.6,
     },
-    VariableCategory.CATEGORY_E: {
+    VariableCategory.E: {
         "psi_0": 1.0,
         "psi_1": 0.9,
         "psi_2": 0.8,
     },
-    VariableCategory.CATEGORY_F: {
+    VariableCategory.F: {
         "psi_0": 0.7,
         "psi_1": 0.7,
         "psi_2": 0.6,
     },
-    VariableCategory.CATEGORY_G: {
+    VariableCategory.G: {
         "psi_0": 0.7,
         "psi_1": 0.5,
         "psi_2": 0.3,
     },
-    VariableCategory.CATEGORY_H: {
+    VariableCategory.H: {
         "psi_0": 0.0,
         "psi_1": 0.0,
         "psi_2": 0.0,
     },
     VariableCategory.SNOW_ABOVE_1000_M: {
         "psi_0": 0.7,
         "psi_1": 0.5,
```

### Comparing `desssign-0.0.2/src/desssign/loads/load_combination_generator/generate_combinations.py` & `desssign-0.0.3/src/desssign/loads/load_combination_generator/generate_combinations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,91 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
-
 from desssign.loads.enums import LoadBehavior
 from desssign.loads.enums import SLSCombination
+from desssign.loads.enums import ULSAlternativeCombination
 from desssign.loads.enums import ULSCombination
 from desssign.loads.enums import VariableCategory
-from desssign.loads.load_combination import DesignLoadCombination
+from desssign.loads.load_case import DesignLoadCase
 from desssign.loads.load_combination_generator.constants import GAMMA_VALUES
 from desssign.loads.load_combination_generator.constants import PSI_FACTORS
 from desssign.loads.load_combination_generator.constants import XI
 
-if TYPE_CHECKING:
-    from desssign.loads.load_case import DesignLoadCase
-
 
 def generate_combination(
-    i: int,
     permanent_cases: list[DesignLoadCase],
     leading_variable_case: DesignLoadCase | None,
     other_variable_cases: list[DesignLoadCase],
     combination: SLSCombination | ULSCombination,
-) -> list[DesignLoadCombination]:
+    alternative_combination: ULSAlternativeCombination | None = None,
+) -> tuple[dict[DesignLoadCase, float], str]:
+    """
+    Generate a combination of load cases according to the limit state and combination type.
+
+    :param permanent_cases: A list of permanent load cases.
+    :param leading_variable_case: The leading variable load case.
+    :param other_variable_cases: A list of other variable load cases.
+    :param combination: Type of SLS or ULS combination.
+    :param alternative_combination: Specifier for the used equation, only required for ULS alternative combinations.
+                                    Either '6.10a' or '6.10b'.
+    :raises AttributeError: If the combination type is unknown.
+    """
     if combination == SLSCombination.CHARACTERISTIC:
         return generate_sls_characteristic_combination(
-            i, permanent_cases, leading_variable_case, other_variable_cases
+            permanent_cases, leading_variable_case, other_variable_cases
         )
 
     if combination == SLSCombination.FREQUENT:
         return generate_sls_frequent_combination(
-            i, permanent_cases, leading_variable_case, other_variable_cases
+            permanent_cases, leading_variable_case, other_variable_cases
         )
 
     if combination == SLSCombination.QUASIPERMANENT:
         return generate_sls_quasipermanent_combination(
-            i, permanent_cases, leading_variable_case, other_variable_cases
+            permanent_cases, leading_variable_case, other_variable_cases
         )
 
     if combination == ULSCombination.BASIC:
         return generate_uls_basic_combination(
-            i, permanent_cases, leading_variable_case, other_variable_cases
+            permanent_cases, leading_variable_case, other_variable_cases
         )
 
     if combination == ULSCombination.ALTERNATIVE:
-        return generate_uls_alternative_combinations(
-            i, permanent_cases, leading_variable_case, other_variable_cases
+        if alternative_combination == ULSAlternativeCombination.REDUCED_VARIABLE:
+            return generate_uls_alternative_a_combination(
+                permanent_cases, leading_variable_case, other_variable_cases
+            )
+
+        if alternative_combination == ULSAlternativeCombination.REDUCED_PERMANENT:
+            return generate_uls_alternative_b_combination(
+                permanent_cases, leading_variable_case, other_variable_cases
+            )
+
+        raise AttributeError(
+            f"Unknown alternative combination: '{alternative_combination}'."
         )
-    else:
-        raise AttributeError(f"Unknown combination: '{combination}'.")
+
+    raise AttributeError(f"Unknown combination: '{combination}'.")
 
 
 def generate_sls_characteristic_combination(
-    i: int,
     permanent_cases: list[DesignLoadCase],
     leading_variable_case: DesignLoadCase | None,
     other_variable_cases: list[DesignLoadCase],
-) -> list[DesignLoadCombination]:
+) -> tuple[dict[DesignLoadCase, float], str]:
+    """
+    Generate a characteristic combination of load cases for serviceability limit state.
+
+    Combination is generated according to equations 6.14 of EN 1990.
+    The combination is normally used for irreversible limit states.
+
+    :param permanent_cases: A list of permanent load cases.
+    :param leading_variable_case: The leading variable load case.
+    :param other_variable_cases: A list of other variable load cases.
+    """
     cases = {}
     key = ""
 
     for case in permanent_cases:
         cases[case] = 1.0
         key += f"{case.label}+"
 
@@ -68,23 +94,32 @@
         key += f"{leading_variable_case.label}+"
 
     for case in other_variable_cases:
         factor = PSI_FACTORS[VariableCategory(case.category)]["psi_0"]
         cases[case] = factor
         key += f"{factor}*{case.label}+"
 
-    return [DesignLoadCombination(f"SLS-Characteristic-{i}", cases, key[:-1])]
+    return cases, key[:-1]
 
 
 def generate_sls_frequent_combination(
-    i: int,
     permanent_cases: list[DesignLoadCase],
     leading_variable_case: DesignLoadCase | None,
     other_variable_cases: list[DesignLoadCase],
-) -> list[DesignLoadCombination]:
+) -> tuple[dict[DesignLoadCase, float], str]:
+    """
+    Generate a frequent combination of load cases for serviceability limit state.
+
+    Combination is generated according to equations 6.15 of EN 1990.
+    The combination is normally used for reversible limit states.
+
+    :param permanent_cases: A list of permanent load cases.
+    :param leading_variable_case: The leading variable load case.
+    :param other_variable_cases: A list of other variable load cases.
+    """
     cases = {}
     key = ""
 
     for case in permanent_cases:
         cases[case] = 1.0
         key += f"{case.label}+"
 
@@ -94,23 +129,32 @@
         key += f"{factor}*{leading_variable_case.label}+"
 
     for case in other_variable_cases:
         factor = PSI_FACTORS[VariableCategory(case.category)]["psi_2"]
         cases[case] = factor
         key += f"{factor}*{case.label}+"
 
-    return [DesignLoadCombination(f"SLS-Frequent-{i}", cases, key[:-1])]
+    return cases, key[:-1]
 
 
 def generate_sls_quasipermanent_combination(
-    i: int,
     permanent_cases: list[DesignLoadCase],
     leading_variable_case: DesignLoadCase | None,
     other_variable_cases: list[DesignLoadCase],
-) -> list[DesignLoadCombination]:
+) -> tuple[dict[DesignLoadCase, float], str]:
+    """
+    Generate a quasipermanent combination of load cases for serviceability limit state.
+
+    Combination is generated according to equations 6.16 of EN 1990.
+    The combination is normally used for long-term effects and the appearance of the structure.
+
+    :param permanent_cases: A list of permanent load cases.
+    :param leading_variable_case: The leading variable load case.
+    :param other_variable_cases: A list of other variable load cases.
+    """
     cases = {}
     key = ""
 
     for case in permanent_cases:
         cases[case] = 1.0
         key += f"{case.label}+"
 
@@ -120,23 +164,31 @@
         key += f"{factor}*{leading_variable_case.label}+"
 
     for case in other_variable_cases:
         factor = PSI_FACTORS[VariableCategory(case.category)]["psi_2"]
         cases[case] = factor
         key += f"{factor}*{case.label}+"
 
-    return [DesignLoadCombination(f"SLS-Frequent-{i}", cases, key[:-1])]
+    return cases, key[:-1]
 
 
 def generate_uls_basic_combination(
-    i: int,
     permanent_cases: list[DesignLoadCase],
     leading_variable_case: DesignLoadCase | None,
     other_variable_cases: list[DesignLoadCase],
-) -> list[DesignLoadCombination]:
+) -> tuple[dict[DesignLoadCase, float], str]:
+    """
+    Generate a basic combination of load cases for ultimate limit state.
+
+    Combination is generated according to equations 6.10 of EN 1990.
+
+    :param permanent_cases: A list of permanent load cases.
+    :param leading_variable_case: The leading variable load case.
+    :param other_variable_cases: A list of other variable load cases.
+    """
     cases = {}
     key = ""
 
     for case in permanent_cases:
         factor = GAMMA_VALUES["Set B"][case.load_type][
             LoadBehavior.UNFAVOURABLE
         ]  # TODO: Favourable?
@@ -154,73 +206,93 @@
         gamma = GAMMA_VALUES["Set B"][case.load_type][
             LoadBehavior.UNFAVOURABLE
         ]  # TODO: Favourable?
         psi = PSI_FACTORS[VariableCategory(case.category)]["psi_0"]
         cases[case] = gamma * psi
         key += f"{gamma}*{psi}*{case.label}+"
 
-    return [DesignLoadCombination(f"ULS-Basic(6.10)-{i}", cases, key[:-1])]
+    return cases, key[:-1]
 
 
-def generate_uls_alternative_combinations(
-    i: int,
+def generate_uls_alternative_a_combination(
     permanent_cases: list[DesignLoadCase],
     leading_variable_case: DesignLoadCase | None,
     other_variable_cases: list[DesignLoadCase],
-) -> list[DesignLoadCombination]:
-    cases_a = {}
-    key_a = ""
+) -> tuple[dict[DesignLoadCase, float], str]:
+    """
+    Generate two alternative combinations of load cases for ultimate limit state.
+
+    Combinations are generated according to equation 6.10a of EN 1990.
+
+    :param permanent_cases: A list of permanent load cases.
+    :param leading_variable_case: The leading variable load case.
+    :param other_variable_cases: A list of other variable load cases.
+    """
+    cases = {}
+    key = ""
 
     for case in permanent_cases:
         gamma = GAMMA_VALUES["Set B"][case.load_type][
             LoadBehavior.UNFAVOURABLE
         ]  # TODO: Favourable?
-        cases_a[case] = gamma
-        key_a += f"{gamma}*{case.label}+"
+        cases[case] = gamma
+        key += f"{gamma}*{case.label}+"
 
     if leading_variable_case is not None:
         gamma = GAMMA_VALUES["Set B"][leading_variable_case.load_type][
             LoadBehavior.UNFAVOURABLE
         ]  # TODO: Favourable?
         psi = PSI_FACTORS[VariableCategory(leading_variable_case.category)]["psi_0"]
-        cases_a[leading_variable_case] = gamma * psi
-        key_a += f"{gamma}*{psi}*{leading_variable_case.label}+"
+        cases[leading_variable_case] = gamma * psi
+        key += f"{gamma}*{psi}*{leading_variable_case.label}+"
 
     for case in other_variable_cases:
         gamma = GAMMA_VALUES["Set B"][case.load_type][
             LoadBehavior.UNFAVOURABLE
         ]  # TODO: Favourable?
         psi = PSI_FACTORS[VariableCategory(case.category)]["psi_0"]
-        cases_a[case] = gamma * psi
-        key_a += f"{gamma}*{psi}*{case.label}+"
+        cases[case] = gamma * psi
+        key += f"{gamma}*{psi}*{case.label}+"
+
+    return cases, key[:-1]
 
-    cases_b = {}
-    key_b = ""
+
+def generate_uls_alternative_b_combination(
+    permanent_cases: list[DesignLoadCase],
+    leading_variable_case: DesignLoadCase | None,
+    other_variable_cases: list[DesignLoadCase],
+) -> tuple[dict[DesignLoadCase, float], str]:
+    """
+    Generate two alternative combinations of load cases for ultimate limit state.
+
+    Combinations are generated according to equation 6.10b of EN 1990.
+
+    :param permanent_cases: A list of permanent load cases.
+    :param leading_variable_case: The leading variable load case.
+    :param other_variable_cases: A list of other variable load cases.
+    """
+    cases = {}
+    key = ""
 
     for case in permanent_cases:
         gamma = GAMMA_VALUES["Set B"][case.load_type][
             LoadBehavior.UNFAVOURABLE
         ]  # TODO: Favourable?
-        cases_b[case] = gamma * XI
-        key_b += f"{XI}*{gamma}*{case.label}+"
+        cases[case] = gamma * XI
+        key += f"{XI}*{gamma}*{case.label}+"
 
     if leading_variable_case is not None:
         gamma = GAMMA_VALUES["Set B"][leading_variable_case.load_type][
             LoadBehavior.UNFAVOURABLE
         ]  # TODO: Favourable?
-        cases_b[leading_variable_case] = gamma
-        key_b += f"{gamma}*{leading_variable_case.label}+"
+        cases[leading_variable_case] = gamma
+        key += f"{gamma}*{leading_variable_case.label}+"
 
     for case in other_variable_cases:
         gamma = GAMMA_VALUES["Set B"][case.load_type][
             LoadBehavior.UNFAVOURABLE
         ]  # TODO: Favourable?
         psi = PSI_FACTORS[VariableCategory(case.category)]["psi_0"]
-        cases_b[case] = gamma * psi
-        key_b += f"{gamma}*{psi}*{case.label}+"
-
-    combinations = [
-        DesignLoadCombination(f"ULS-Alternative(6.10a)-{i}", cases_a, key_a[:-1]),
-        DesignLoadCombination(f"ULS-Alternative(6.10b)-{i}", cases_b, key_b[:-1]),
-    ]
+        cases[case] = gamma * psi
+        key += f"{gamma}*{psi}*{case.label}+"
 
-    return combinations
+    return cases, key[:-1]
```

### Comparing `desssign-0.0.2/src/desssign/loads/load_group.py` & `desssign-0.0.3/src/desssign/loads/load_case_group.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,34 +5,41 @@
 
 from desssign.loads.enums import LoadCaseRelation
 
 if TYPE_CHECKING:
     from desssign.loads.load_case import DesignLoadCase
 
 
-class LoadGroup:
+class DesignLoadCaseGroup:
+    """
+    Class representing a group of load cases and relation between them.
+
+    :ivar load_cases: List of :class:`DesignLoad` instances.
+    :ivar load_case_relation: Relation between :class:`DesignLoad` instances.
+    """
+
     def __init__(
         self,
         load_cases: list[DesignLoadCase],
         load_case_relation: str | LoadCaseRelation = LoadCaseRelation.STANDARD,
     ) -> None:
         """
-        Init the LoadGroup class.
+        Init the DesignLoadCaseGroup class.
 
         :param load_cases: List of :class:`DesignLoadCase` instances.
         :param load_case_relation: Relation between :class:`DesignLoadCase` instances.
                                    Possible values are ['together', 'standard', 'exclusive'].
         """
         self.load_cases = load_cases
         self.load_case_relation = LoadCaseRelation(load_case_relation)
 
     def __repr__(self) -> str:
-        """Return a string representation of the LoadGroup object."""
+        """Return a string representation of the DesignLoadCaseGroup object."""
         return (
-            f"LoadGroup("
+            f"DesignLoadCaseGroup("
             f"load_cases={self.load_cases}, "
             f"load_case_relation={self.load_case_relation}"
             f")"
         )
 
     @property
     def number_of_load_cases(self) -> int:
@@ -56,10 +63,8 @@
                 for comb in combinations(self.load_cases, i)
             ]
         if self.load_case_relation == LoadCaseRelation.EXCLUSIVE:
             comb = [[comb] for comb in self.load_cases]
             comb.insert(0, [])
             return comb
         else:
-            raise AttributeError(
-                f"Invalid load case relation: {self.load_case_relation}"
-            )
+            raise ValueError(f"Invalid load case relation: {self.load_case_relation}")
```

### Comparing `desssign-0.0.2/src/desssign/utils.py` & `desssign-0.0.3/src/desssign/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,12 +14,12 @@
     lists found. Non-list items are appended directly to the output list.
 
     :param mixed_list: A list potentially containing nested lists along with other items.
     :return: A single, flattened list containing all elements from the input, preserving order.
     """
     flat_list = []
     for item in mixed_list:
-        if isinstance(item, list):  # Check if the item is a list
-            flat_list.extend(item)  # Extend flat_list with the items of the inner list
+        if isinstance(item, (list, tuple)):  # Check if the item is a list or tuple
+            flat_list.extend(flatten_list(item))  # Recursively flatten and extend
         else:
             flat_list.append(item)  # Append the item directly if it's not a list
     return flat_list
```

### Comparing `desssign-0.0.2/src/desssign/wood/strength_classes.py` & `desssign-0.0.3/src/desssign/wood/strength_classes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,392 +1,392 @@
 """
-This module contains mechanical properties of wood according to ČSN EN 338:2016.
+The module contains mechanical properties of wood according to ČSN EN 338:2016.
 
-E_m0mean: mean characteristic value of modulus of elasticity in bending parallel to grain (in kN/mm2)
-E_t0,mean: mean characteristic value of modulus of elasticity in tension parallel to grain (in kN/mm2)
-E_m0k: 5-percentile characteristic value of modulus of elasticity in bending parallel to grain (in kN/mm2)
-E_t0k: 5-percentile characteristic value of modulus of elasticity in tension parallel to grain (in kN/mm2)
-E_m90mean: mean characteristic value of modulus of elasticity in bending perpendicular to grain (in kN/mm2)
-E_t90mean: mean characteristic value of modulus of elasticity in tension perpendicular to grain (in kN/mm2)
-f_c0k: 5-percentile characteristic value of compressive strength parallel to grain (in N/mm2)
-f_c90k: 5-percentile characteristic value of compressive strength perpendicular to grain (in N/mm2)
-f_mk: 5-percentile characteristic value of bending strength (in N/mm2)
-f_t0k: 5-percentile characteristic value of tensile strength parallel to grain (in N/mm2)
-f_t90k: 5-percentile characteristic value of tensile strength perpendicular to grain (in N/mm2)
-f_vk: 5-percentile characteristic value of shear strength (in N/mm2)
-G_mean: mean characteristic value of shear modulus (in kN/mm2)
+E_m0mean: mean characteristic value of modulus of elasticity in bending parallel to grain (in N/m2)
+E_t0,mean: mean characteristic value of modulus of elasticity in tension parallel to grain (in N/m2)
+E_m0k: 5-percentile characteristic value of modulus of elasticity in bending parallel to grain (in N/m2)
+E_t0k: 5-percentile characteristic value of modulus of elasticity in tension parallel to grain (in N/m2)
+E_m90mean: mean characteristic value of modulus of elasticity in bending perpendicular to grain (in N/m2)
+E_t90mean: mean characteristic value of modulus of elasticity in tension perpendicular to grain (in N/m2)
+f_c0k: 5-percentile characteristic value of compressive strength parallel to grain (in N/m2)
+f_c90k: 5-percentile characteristic value of compressive strength perpendicular to grain (in N/m2)
+f_mk: 5-percentile characteristic value of bending strength (in N/m2)
+f_t0k: 5-percentile characteristic value of tensile strength parallel to grain (in N/m2)
+f_t90k: 5-percentile characteristic value of tensile strength perpendicular to grain (in N/m2)
+f_vk: 5-percentile characteristic value of shear strength (in N/m2)
+G_mean: mean characteristic value of shear modulus (in N/m2)
 rho_k: 5-percentile characteristic value of density (in kg/m3)
 rho_mean: mean characteristic value of density (in kg/m3)
 """
 
 SOFTWOOD_STRENGTH_CLASSES = {
     "C14": {
-        "f_mk": 14.0,
-        "f_t0k": 7.2,
-        "f_t90k": 0.4,
-        "f_c0k": 16.0,
-        "f_c90k": 2.0,
-        "f_vk": 3.0,
-        "E_m0mean": 7.0,
-        "E_m0k": 4.7,
-        "E_m90mean": 0.23,
-        "G_mean": 0.44,
+        "f_mk": 14.0e6,
+        "f_t0k": 7.2e6,
+        "f_t90k": 0.4e6,
+        "f_c0k": 16.0e6,
+        "f_c90k": 2.0e6,
+        "f_vk": 3.0e6,
+        "E_m0mean": 7.0e9,
+        "E_m0k": 4.7e9,
+        "E_m90mean": 0.23e9,
+        "G_mean": 0.44e9,
         "rho_k": 290.0,
         "rho_mean": 350.0,
     },
     "C16": {
-        "f_mk": 16.0,
-        "f_t0k": 8.5,
-        "f_t90k": 0.4,
-        "f_c0k": 17,
-        "f_c90k": 2.2,
-        "f_vk": 3.2,
-        "E_m0mean": 8.0,
-        "E_m0k": 5.4,
-        "E_m90mean": 0.27,
-        "G_mean": 0.5,
+        "f_mk": 16.0e6,
+        "f_t0k": 8.5e6,
+        "f_t90k": 0.4e6,
+        "f_c0k": 17.0e6,
+        "f_c90k": 2.2e6,
+        "f_vk": 3.2e6,
+        "E_m0mean": 8.0e9,
+        "E_m0k": 5.4e9,
+        "E_m90mean": 0.27e9,
+        "G_mean": 0.5e9,
         "rho_k": 310.0,
         "rho_mean": 370.0,
     },
     "C18": {
-        "f_mk": 18.0,
-        "f_t0k": 10.0,
-        "f_t90k": 0.4,
-        "f_c0k": 18.0,
-        "f_c90k": 2.2,
-        "f_vk": 3.4,
-        "E_m0mean": 9.0,
-        "E_m0k": 6.0,
-        "E_m90mean": 0.3,
-        "G_mean": 0.56,
+        "f_mk": 18.0e6,
+        "f_t0k": 10.0e6,
+        "f_t90k": 0.4e6,
+        "f_c0k": 18.0e6,
+        "f_c90k": 2.2e6,
+        "f_vk": 3.4e6,
+        "E_m0mean": 9.0e9,
+        "E_m0k": 6.0e9,
+        "E_m90mean": 0.3e9,
+        "G_mean": 0.56e9,
         "rho_k": 320.0,
         "rho_mean": 380.0,
     },
     "C20": {
-        "f_mk": 20.0,
-        "f_t0k": 11.5,
-        "f_t90k": 0.4,
-        "f_c0k": 19.0,
-        "f_c90k": 2.3,
-        "f_vk": 3.6,
-        "E_m0mean": 9.5,
-        "E_m0k": 6.4,
-        "E_m90mean": 0.32,
-        "G_mean": 0.59,
+        "f_mk": 20.0e6,
+        "f_t0k": 11.5e6,
+        "f_t90k": 0.4e6,
+        "f_c0k": 19.0e6,
+        "f_c90k": 2.3e6,
+        "f_vk": 3.6e6,
+        "E_m0mean": 9.5e9,
+        "E_m0k": 6.4e9,
+        "E_m90mean": 0.32e9,
+        "G_mean": 0.59e9,
         "rho_k": 330.0,
         "rho_mean": 400.0,
     },
     "C22": {
-        "f_mk": 22.0,
-        "f_t0k": 13.0,
-        "f_t90k": 0.4,
-        "f_c0k": 20.0,
-        "f_c90k": 2.4,
-        "f_vk": 3.8,
-        "E_m0mean": 10.0,
-        "E_m0k": 6.7,
-        "E_m90mean": 0.33,
-        "G_mean": 0.63,
+        "f_mk": 22.0e6,
+        "f_t0k": 13.0e6,
+        "f_t90k": 0.4e6,
+        "f_c0k": 20.0e6,
+        "f_c90k": 2.4e6,
+        "f_vk": 3.8e6,
+        "E_m0mean": 10.0e9,
+        "E_m0k": 6.7e9,
+        "E_m90mean": 0.33e9,
+        "G_mean": 0.63e9,
         "rho_k": 340.0,
         "rho_mean": 410.0,
     },
     "C24": {
-        "f_mk": 24.0,
-        "f_t0k": 14.5,
-        "f_t90k": 0.4,
-        "f_c0k": 21.0,
-        "f_c90k": 2.5,
-        "f_vk": 4.0,
-        "E_m0mean": 11.0,
-        "E_m0k": 7.4,
-        "E_m90mean": 0.37,
-        "G_mean": 0.69,
+        "f_mk": 24.0e6,
+        "f_t0k": 14.5e6,
+        "f_t90k": 0.4e6,
+        "f_c0k": 21.0e6,
+        "f_c90k": 2.5e6,
+        "f_vk": 4.0e6,
+        "E_m0mean": 11.0e9,
+        "E_m0k": 7.4e9,
+        "E_m90mean": 0.37e9,
+        "G_mean": 0.69e9,
         "rho_k": 350.0,
         "rho_mean": 420.0,
     },
     "C27": {
-        "f_mk": 27.0,
-        "f_t0k": 16.5,
-        "f_t90k": 0.4,
-        "f_c0k": 22.0,
-        "f_c90k": 2.5,
-        "f_vk": 4.0,
-        "E_m0mean": 11.5,
-        "E_m0k": 7.7,
-        "E_m90mean": 0.38,
-        "G_mean": 0.72,
+        "f_mk": 27.0e6,
+        "f_t0k": 16.5e6,
+        "f_t90k": 0.4e6,
+        "f_c0k": 22.0e6,
+        "f_c90k": 2.5e6,
+        "f_vk": 4.0e6,
+        "E_m0mean": 11.5e9,
+        "E_m0k": 7.7e9,
+        "E_m90mean": 0.38e9,
+        "G_mean": 0.72e9,
         "rho_k": 360.0,
         "rho_mean": 430.0,
     },
     "C30": {
-        "f_mk": 30.0,
-        "f_t0k": 19.0,
-        "f_t90k": 0.4,
-        "f_c0k": 24.0,
-        "f_c90k": 2.7,
-        "f_vk": 4.0,
-        "E_m0mean": 12.0,
-        "E_m0k": 8.0,
-        "E_m90mean": 0.4,
-        "G_mean": 0.75,
+        "f_mk": 30.0e6,
+        "f_t0k": 19.0e6,
+        "f_t90k": 0.4e6,
+        "f_c0k": 24.0e6,
+        "f_c90k": 2.7e6,
+        "f_vk": 4.0e6,
+        "E_m0mean": 12.0e9,
+        "E_m0k": 8.0e9,
+        "E_m90mean": 0.4e9,
+        "G_mean": 0.75e9,
         "rho_k": 380.0,
         "rho_mean": 460.0,
     },
     "C35": {
-        "f_mk": 35.0,
-        "f_t0k": 22.5,
-        "f_t90k": 0.4,
-        "f_c0k": 25.0,
-        "f_c90k": 2.7,
-        "f_vk": 4.0,
-        "E_m0mean": 13.0,
-        "E_m0k": 8.7,
-        "E_m90mean": 0.43,
-        "G_mean": 0.81,
+        "f_mk": 35.0e6,
+        "f_t0k": 22.5e6,
+        "f_t90k": 0.4e6,
+        "f_c0k": 25.0e6,
+        "f_c90k": 2.7e6,
+        "f_vk": 4.0e6,
+        "E_m0mean": 13.0e9,
+        "E_m0k": 8.7e9,
+        "E_m90mean": 0.43e9,
+        "G_mean": 0.81e9,
         "rho_k": 390.0,
         "rho_mean": 470.0,
     },
     "C40": {
-        "f_mk": 40.0,
-        "f_t0k": 26.0,
-        "f_t90k": 0.4,
-        "f_c0k": 27.0,
-        "f_c90k": 2.8,
-        "f_vk": 4.0,
-        "E_m0mean": 14.0,
-        "E_m0k": 9.4,
-        "E_m90mean": 0.47,
-        "G_mean": 0.88,
+        "f_mk": 40.0e6,
+        "f_t0k": 26.0e6,
+        "f_t90k": 0.4e6,
+        "f_c0k": 27.0e6,
+        "f_c90k": 2.8e6,
+        "f_vk": 4.0e6,
+        "E_m0mean": 14.0e9,
+        "E_m0k": 9.4e9,
+        "E_m90mean": 0.47e9,
+        "G_mean": 0.88e9,
         "rho_k": 400.0,
         "rho_mean": 480.0,
     },
     "C45": {
-        "f_mk": 45.0,
-        "f_t0k": 30.0,
-        "f_t90k": 0.4,
-        "f_c0k": 29.0,
-        "f_c90k": 2.9,
-        "f_vk": 4.0,
-        "E_m0mean": 15.0,
-        "E_m0k": 10.1,
-        "E_m90mean": 0.5,
-        "G_mean": 0.94,
+        "f_mk": 45.0e6,
+        "f_t0k": 30.0e6,
+        "f_t90k": 0.4e6,
+        "f_c0k": 29.0e6,
+        "f_c90k": 2.9e6,
+        "f_vk": 4.0e6,
+        "E_m0mean": 15.0e9,
+        "E_m0k": 10.1e9,
+        "E_m90mean": 0.5e9,
+        "G_mean": 0.94e9,
         "rho_k": 410.0,
         "rho_mean": 490.0,
     },
     "C50": {
-        "f_mk": 50.0,
-        "f_t0k": 33.5,
-        "f_t90k": 0.4,
-        "f_c0k": 30.0,
-        "f_c90k": 3.0,
-        "f_vk": 4.0,
-        "E_m0mean": 16.0,
-        "E_m0k": 10.7,
-        "E_m90mean": 0.53,
-        "G_mean": 1.0,
+        "f_mk": 50.0e6,
+        "f_t0k": 33.5e6,
+        "f_t90k": 0.4e6,
+        "f_c0k": 30.0e6,
+        "f_c90k": 3.0e6,
+        "f_vk": 4.0e6,
+        "E_m0mean": 16.0e9,
+        "E_m0k": 10.7e9,
+        "E_m90mean": 0.53e9,
+        "G_mean": 1.0e9,
         "rho_k": 430.0,
         "rho_mean": 520.0,
     },
 }
 
 
 HARDWOOD_STRENGTH_CLASSES = {
     "D18": {
-        "f_mk": 18.0,
-        "f_t0k": 11.0,
-        "f_t90k": 0.6,
-        "f_c0k": 18.0,
-        "f_c90k": 4.8,
-        "f_vk": 3.5,
-        "E_m0mean": 9.5,
-        "E_m0k": 8.0,
-        "E_m90mean": 0.63,
-        "G_mean": 0.59,
+        "f_mk": 18.0e6,
+        "f_t0k": 11.0e6,
+        "f_t90k": 0.6e6,
+        "f_c0k": 18.0e6,
+        "f_c90k": 4.8e6,
+        "f_vk": 3.5e6,
+        "E_m0mean": 9.5e9,
+        "E_m0k": 8.0e9,
+        "E_m90mean": 0.63e9,
+        "G_mean": 0.59e9,
         "rho_k": 475.0,
         "rho_mean": 570.0,
     },
     "D24": {
-        "f_mk": 24.0,
-        "f_t0k": 14.0,
-        "f_t90k": 0.6,
-        "f_c0k": 21.0,
-        "f_c90k": 4.9,
-        "f_vk": 3.7,
-        "E_m0mean": 10.0,
-        "E_m0k": 8.4,
-        "E_m90mean": 0.67,
-        "G_mean": 0.63,
+        "f_mk": 24.0e6,
+        "f_t0k": 14.0e6,
+        "f_t90k": 0.6e6,
+        "f_c0k": 21.0e6,
+        "f_c90k": 4.9e6,
+        "f_vk": 3.7e6,
+        "E_m0mean": 10.0e9,
+        "E_m0k": 8.4e9,
+        "E_m90mean": 0.67e9,
+        "G_mean": 0.63e9,
         "rho_k": 485.0,
         "rho_mean": 580.0,
     },
     "D27": {
-        "f_mk": 27.0,
-        "f_t0k": 16.0,
-        "f_t90k": 0.6,
-        "f_c0k": 22.0,
-        "f_c90k": 5.1,
-        "f_vk": 3.8,
-        "E_m0mean": 10.5,
-        "E_m0k": 8.8,
-        "E_m90mean": 0.7,
-        "G_mean": 0.66,
+        "f_mk": 27.0e6,
+        "f_t0k": 16.0e6,
+        "f_t90k": 0.6e6,
+        "f_c0k": 22.0e6,
+        "f_c90k": 5.1e6,
+        "f_vk": 3.8e6,
+        "E_m0mean": 10.5e9,
+        "E_m0k": 8.8e9,
+        "E_m90mean": 0.7e9,
+        "G_mean": 0.66e9,
         "rho_k": 510.0,
         "rho_mean": 610.0,
     },
     "D30": {
-        "f_mk": 30.0,
-        "f_t0k": 18.0,
-        "f_t90k": 0.6,
-        "f_c0k": 24.0,
-        "f_c90k": 5.3,
-        "f_vk": 3.9,
-        "E_m0mean": 11.0,
-        "E_m0k": 9.2,
-        "E_m90mean": 0.73,
-        "G_mean": 0.69,
+        "f_mk": 30.0e6,
+        "f_t0k": 18.0e6,
+        "f_t90k": 0.6e6,
+        "f_c0k": 24.0e6,
+        "f_c90k": 5.3e6,
+        "f_vk": 3.9e6,
+        "E_m0mean": 11.0e9,
+        "E_m0k": 9.2e9,
+        "E_m90mean": 0.73e9,
+        "G_mean": 0.69e9,
         "rho_k": 530.0,
         "rho_mean": 640.0,
     },
     "D35": {
-        "f_mk": 35.0,
-        "f_t0k": 21.0,
-        "f_t90k": 0.6,
-        "f_c0k": 25.0,
-        "f_c90k": 5.4,
-        "f_vk": 4.1,
-        "E_m0mean": 12.0,
-        "E_m0k": 10.1,
-        "E_m90mean": 0.8,
-        "G_mean": 0.75,
+        "f_mk": 35.0e6,
+        "f_t0k": 21.0e6,
+        "f_t90k": 0.6e6,
+        "f_c0k": 25.0e6,
+        "f_c90k": 5.4e6,
+        "f_vk": 4.1e6,
+        "E_m0mean": 12.0e9,
+        "E_m0k": 10.1e9,
+        "E_m90mean": 0.8e9,
+        "G_mean": 0.75e9,
         "rho_k": 540.0,
         "rho_mean": 650.0,
     },
     "D40": {
-        "f_mk": 40.0,
-        "f_t0k": 24.0,
-        "f_t90k": 0.6,
-        "f_c0k": 27.0,
-        "f_c90k": 5.5,
-        "f_vk": 4.2,
-        "E_m0mean": 13.0,
-        "E_m0k": 10.9,
-        "E_m90mean": 0.87,
-        "G_mean": 0.81,
+        "f_mk": 40.0e6,
+        "f_t0k": 24.0e6,
+        "f_t90k": 0.6e6,
+        "f_c0k": 27.0e6,
+        "f_c90k": 5.5e6,
+        "f_vk": 4.2e6,
+        "E_m0mean": 13.0e9,
+        "E_m0k": 10.9e9,
+        "E_m90mean": 0.87e9,
+        "G_mean": 0.81e9,
         "rho_k": 550.0,
         "rho_mean": 660.0,
     },
     "D45": {
-        "f_mk": 45.0,
-        "f_t0k": 27.0,
-        "f_t90k": 0.6,
-        "f_c0k": 29.0,
-        "f_c90k": 5.8,
-        "f_vk": 4.4,
-        "E_m0mean": 13.5,
-        "E_m0k": 11.3,
-        "E_m90mean": 0.9,
-        "G_mean": 0.84,
+        "f_mk": 45.0e6,
+        "f_t0k": 27.0e6,
+        "f_t90k": 0.6e6,
+        "f_c0k": 29.0e6,
+        "f_c90k": 5.8e6,
+        "f_vk": 4.4e6,
+        "E_m0mean": 13.5e9,
+        "E_m0k": 11.3e9,
+        "E_m90mean": 0.9e9,
+        "G_mean": 0.84e9,
         "rho_k": 580.0,
         "rho_mean": 700.0,
     },
     "D50": {
-        "f_mk": 50.0,
-        "f_t0k": 30.0,
-        "f_t90k": 0.6,
-        "f_c0k": 30.0,
-        "f_c90k": 6.2,
-        "f_vk": 4.5,
-        "E_m0mean": 14.0,
-        "E_m0k": 11.8,
-        "E_m90mean": 0.93,
-        "G_mean": 0.88,
+        "f_mk": 50.0e6,
+        "f_t0k": 30.0e6,
+        "f_t90k": 0.6e6,
+        "f_c0k": 30.0e6,
+        "f_c90k": 6.2e6,
+        "f_vk": 4.5e6,
+        "E_m0mean": 14.0e9,
+        "E_m0k": 11.8e9,
+        "E_m90mean": 0.93e9,
+        "G_mean": 0.88e9,
         "rho_k": 620.0,
         "rho_mean": 740.0,
     },
     "D55": {
-        "f_mk": 55.0,
-        "f_t0k": 33.0,
-        "f_t90k": 0.6,
-        "f_c0k": 32.0,
-        "f_c90k": 6.6,
-        "f_vk": 4.7,
-        "E_m0mean": 15.5,
-        "E_m0k": 13.0,
-        "E_m90mean": 1.03,
-        "G_mean": 0.97,
+        "f_mk": 55.0e6,
+        "f_t0k": 33.0e6,
+        "f_t90k": 0.6e6,
+        "f_c0k": 32.0e6,
+        "f_c90k": 6.6e6,
+        "f_vk": 4.7e6,
+        "E_m0mean": 15.5e9,
+        "E_m0k": 13.0e9,
+        "E_m90mean": 1.03e9,
+        "G_mean": 0.97e9,
         "rho_k": 660.0,
         "rho_mean": 790.0,
     },
     "D60": {
-        "f_mk": 60.0,
-        "f_t0k": 36.0,
-        "f_t90k": 0.6,
-        "f_c0k": 33.0,
-        "f_c90k": 10.5,
-        "f_vk": 4.8,
-        "E_m0mean": 17.0,
-        "E_m0k": 14.3,
-        "E_m90mean": 1.13,
-        "G_mean": 1.06,
+        "f_mk": 60.0e6,
+        "f_t0k": 36.0e6,
+        "f_t90k": 0.6e6,
+        "f_c0k": 33.0e6,
+        "f_c90k": 10.5e6,
+        "f_vk": 4.8e6,
+        "E_m0mean": 17.0e9,
+        "E_m0k": 14.3e9,
+        "E_m90mean": 1.13e9,
+        "G_mean": 1.06e9,
         "rho_k": 700.0,
         "rho_mean": 840.0,
     },
     "D65": {
-        "f_mk": 65.0,
-        "f_t0k": 39.0,
-        "f_t90k": 0.6,
-        "f_c0k": 35.0,
-        "f_c90k": 11.3,
-        "f_vk": 5.0,
-        "E_m0mean": 18.5,
-        "E_m0k": 15.5,
-        "E_m90mean": 1.23,
-        "G_mean": 1.16,
+        "f_mk": 65.0e6,
+        "f_t0k": 39.0e6,
+        "f_t90k": 0.6e6,
+        "f_c0k": 35.0e6,
+        "f_c90k": 11.3e6,
+        "f_vk": 5.0e6,
+        "E_m0mean": 18.5e9,
+        "E_m0k": 15.5e9,
+        "E_m90mean": 1.23e9,
+        "G_mean": 1.16e9,
         "rho_k": 750.0,
         "rho_mean": 900.0,
     },
     "D70": {
-        "f_mk": 70.0,
-        "f_t0k": 42.0,
-        "f_t90k": 0.6,
-        "f_c0k": 36.0,
-        "f_c90k": 12.0,
-        "f_vk": 5.0,
-        "E_m0mean": 20.0,
-        "E_m0k": 16.8,
-        "E_m90mean": 1.33,
-        "G_mean": 1.25,
+        "f_mk": 70.0e6,
+        "f_t0k": 42.0e6,
+        "f_t90k": 0.6e6,
+        "f_c0k": 36.0e6,
+        "f_c90k": 12.0e6,
+        "f_vk": 5.0e6,
+        "E_m0mean": 20.0e9,
+        "E_m0k": 16.8e9,
+        "E_m90mean": 1.33e9,
+        "G_mean": 1.25e9,
         "rho_k": 800.0,
         "rho_mean": 960.0,
     },
     "D75": {
-        "f_mk": 75.0,
-        "f_t0k": 45.0,
-        "f_t90k": 0.6,
-        "f_c0k": 37.0,
-        "f_c90k": 12.8,
-        "f_vk": 5.0,
-        "E_m0mean": 22.0,
-        "E_m0k": 18.5,
-        "E_m90mean": 1.47,
-        "G_mean": 1.38,
+        "f_mk": 75.0e6,
+        "f_t0k": 45.0e6,
+        "f_t90k": 0.6e6,
+        "f_c0k": 37.0e6,
+        "f_c90k": 12.8e6,
+        "f_vk": 5.0e6,
+        "E_m0mean": 22.0e9,
+        "E_m0k": 18.5e9,
+        "E_m90mean": 1.47e9,
+        "G_mean": 1.38e9,
         "rho_k": 850.0,
         "rho_mean": 1020.0,
     },
     "D80": {
-        "f_mk": 80.0,
-        "f_t0k": 48.0,
-        "f_t90k": 0.6,
-        "f_c0k": 38.0,
-        "f_c90k": 13.5,
-        "f_vk": 5.0,
-        "E_m0mean": 24.0,
-        "E_m0k": 20.2,
-        "E_m90mean": 1.6,
-        "G_mean": 1.5,
+        "f_mk": 80.0e6,
+        "f_t0k": 48.0e6,
+        "f_t90k": 0.6e6,
+        "f_c0k": 38.0e6,
+        "f_c90k": 13.5e6,
+        "f_vk": 5.0e6,
+        "E_m0mean": 24.0e9,
+        "E_m0k": 20.2e9,
+        "E_m90mean": 1.6e9,
+        "G_mean": 1.5e9,
         "rho_k": 900.0,
         "rho_mean": 1080.0,
     },
 }
 
 WOOD_STRENGTH_CLASSES = {**SOFTWOOD_STRENGTH_CLASSES, **HARDWOOD_STRENGTH_CLASSES}
```

### Comparing `desssign-0.0.2/PKG-INFO` & `desssign-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desssign
-Version: 0.0.2
+Version: 0.0.3
 Summary: desssign
 Home-page: https://github.com/DanBeranek/desssign
 License: MIT
 Author: Daniel Beranek
 Author-email: daniel.beraanek@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aenum (>=3.1.15,<4.0.0)
 Requires-Dist: click (>=8.0.1)
-Requires-Dist: framesss (>=0.0.2,<0.0.3)
+Requires-Dist: framesss (>=0.0.3,<0.0.4)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Project-URL: Changelog, https://github.com/DanBeranek/desssign/releases
 Project-URL: Documentation, https://DanBeranek.github.io/desssign
 Project-URL: Repository, https://github.com/DanBeranek/desssign
 Description-Content-Type: text/markdown
 
 # desssign
```

