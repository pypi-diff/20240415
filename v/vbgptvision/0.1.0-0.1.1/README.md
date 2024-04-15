# Comparing `tmp/vbgptvision-0.1.0.tar.gz` & `tmp/vbgptvision-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbgptvision-0.1.0.tar", max compression
+gzip compressed data, was "vbgptvision-0.1.1.tar", max compression
```

## Comparing `vbgptvision-0.1.0.tar` & `vbgptvision-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-09 11:34:23.144533 vbgptvision-0.1.0/README.md
--rw-r--r--   0        0        0      337 2024-04-15 09:50:58.912987 vbgptvision-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 11:34:23.144487 vbgptvision-0.1.0/vbgptvision/__init__.py
--rw-r--r--   0        0        0       53 2024-04-09 13:31:23.783555 vbgptvision-0.1.0/vbgptvision/__main__.py
--rw-r--r--   0        0        0     1236 2024-04-15 09:11:59.351303 vbgptvision-0.1.0/vbgptvision/choice_option.py
--rw-r--r--   0        0        0     2596 2024-04-15 09:04:33.257721 vbgptvision-0.1.0/vbgptvision/functions.py
--rw-r--r--   0        0        0     1357 2024-04-15 09:43:29.433315 vbgptvision-0.1.0/vbgptvision/main.py
--rw-r--r--   0        0        0     7756 2024-04-15 09:04:31.092344 vbgptvision-0.1.0/vbgptvision/prompts.py
--rw-r--r--   0        0        0      244 1970-01-01 00:00:00.000000 vbgptvision-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-09 11:34:23.144533 vbgptvision-0.1.1/README.md
+-rw-r--r--   0        0        0      354 2024-04-15 11:00:23.884477 vbgptvision-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 11:34:23.144487 vbgptvision-0.1.1/vbgptvision/__init__.py
+-rw-r--r--   0        0        0       53 2024-04-09 13:31:23.783555 vbgptvision-0.1.1/vbgptvision/__main__.py
+-rw-r--r--   0        0        0     1236 2024-04-15 09:11:59.351303 vbgptvision-0.1.1/vbgptvision/choice_option.py
+-rw-r--r--   0        0        0     2596 2024-04-15 09:04:33.257721 vbgptvision-0.1.1/vbgptvision/functions.py
+-rw-r--r--   0        0        0     1353 2024-04-15 11:00:13.825860 vbgptvision-0.1.1/vbgptvision/main.py
+-rw-r--r--   0        0        0     7756 2024-04-15 09:04:31.092344 vbgptvision-0.1.1/vbgptvision/prompts.py
+-rw-r--r--   0        0        0      333 1970-01-01 00:00:00.000000 vbgptvision-0.1.1/PKG-INFO
```

### Comparing `vbgptvision-0.1.0/vbgptvision/choice_option.py` & `vbgptvision-0.1.1/vbgptvision/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbgptvision-0.1.0/vbgptvision/functions.py` & `vbgptvision-0.1.1/vbgptvision/functions.py`

 * *Files identical despite different names*

### Comparing `vbgptvision-0.1.0/vbgptvision/main.py` & `vbgptvision-0.1.1/vbgptvision/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,26 +17,26 @@
     required=True,
     multiple=True,
     help="Path to the image file",
 )
 @click.option(
     "-p",
     "--prompt",
+    cls=ChoiceOption,
     type=click.Choice(
         [
             "assertion_reason",
             "mcq",
             "mcq_solution",
             "subjective",
             "match",
             "comprehension",
             "answer",
             "prompt",
         ],
-        cls=ChoiceOption,
         case_sensitive=False,
         prompt=True),
     default=2,
     show_default=True,
     help="Prompt to use for the completion",
 )
 def main(image, prompt):
```

### Comparing `vbgptvision-0.1.0/vbgptvision/prompts.py` & `vbgptvision-0.1.1/vbgptvision/prompts.py`

 * *Files identical despite different names*

