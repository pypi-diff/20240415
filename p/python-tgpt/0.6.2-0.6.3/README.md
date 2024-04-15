# Comparing `tmp/python_tgpt-0.6.2.tar.gz` & `tmp/python_tgpt-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_tgpt-0.6.2.tar", last modified: Sat Apr 13 16:38:00 2024, max compression
+gzip compressed data, was "python_tgpt-0.6.3.tar", last modified: Mon Apr 15 09:54:57 2024, max compression
```

## Comparing `python_tgpt-0.6.2.tar` & `python_tgpt-0.6.3.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.707208 python_tgpt-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19666 2024-04-13 16:38:00.707208 python_tgpt-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16787 2024-04-13 16:38:00.000000 python_tgpt-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 16:38:00.707208 python_tgpt-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.695208 python_tgpt-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.695208 python_tgpt-0.6.2/src/pytgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.695208 python_tgpt-0.6.2/src/pytgpt/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13004 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/api/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.695208 python_tgpt-0.6.2/src/pytgpt/blackboxai/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/blackboxai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/blackboxai/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    78689 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.699208 python_tgpt-0.6.2/src/pytgpt/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/gemini/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.699208 python_tgpt-0.6.2/src/pytgpt/gpt4all/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/gpt4all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/gpt4all/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.699208 python_tgpt-0.6.2/src/pytgpt/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/gpt4free/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/gpt4free/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/gpt4free/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.699208 python_tgpt-0.6.2/src/pytgpt/groq/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/groq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/groq/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.699208 python_tgpt-0.6.2/src/pytgpt/imager/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/imager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/imager/imager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.699208 python_tgpt-0.6.2/src/pytgpt/koboldai/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/koboldai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/koboldai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.699208 python_tgpt-0.6.2/src/pytgpt/leo/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/leo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/leo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.699208 python_tgpt-0.6.2/src/pytgpt/llama2/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/llama2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/llama2/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.699208 python_tgpt-0.6.2/src/pytgpt/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/openai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.699208 python_tgpt-0.6.2/src/pytgpt/opengpt/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/opengpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/opengpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.699208 python_tgpt-0.6.2/src/pytgpt/perplexity/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/perplexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/perplexity/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.703208 python_tgpt-0.6.2/src/pytgpt/phind/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/phind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/phind/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.703208 python_tgpt-0.6.2/src/pytgpt/poe/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/poe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/poe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    23825 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.703208 python_tgpt-0.6.2/src/pytgpt/webchatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/webchatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/src/pytgpt/webchatgpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.707208 python_tgpt-0.6.2/src/python_tgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19666 2024-04-13 16:38:00.000000 python_tgpt-0.6.2/src/python_tgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-13 16:38:00.000000 python_tgpt-0.6.2/src/python_tgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:38:00.000000 python_tgpt-0.6.2/src/python_tgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-13 16:38:00.000000 python_tgpt-0.6.2/src/python_tgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-13 16:38:00.000000 python_tgpt-0.6.2/src/python_tgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 16:38:00.000000 python_tgpt-0.6.2/src/python_tgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:00.707208 python_tgpt-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_blackboxai.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_imager.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_koboldai.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_leo.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_opengpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_phind.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-13 16:37:30.000000 python_tgpt-0.6.2/tests/test_webchatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.125254 python_tgpt-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19666 2024-04-15 09:54:57.125254 python_tgpt-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16787 2024-04-15 09:54:56.000000 python_tgpt-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:54:57.125254 python_tgpt-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.109254 python_tgpt-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.113254 python_tgpt-0.6.3/src/pytgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.113254 python_tgpt-0.6.3/src/pytgpt/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12207 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/api/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.113254 python_tgpt-0.6.3/src/pytgpt/blackboxai/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/blackboxai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/blackboxai/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80577 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.113254 python_tgpt-0.6.3/src/pytgpt/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/gemini/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.113254 python_tgpt-0.6.3/src/pytgpt/gpt4all/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/gpt4all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/gpt4all/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.113254 python_tgpt-0.6.3/src/pytgpt/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/gpt4free/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/gpt4free/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/gpt4free/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.113254 python_tgpt-0.6.3/src/pytgpt/groq/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/groq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/groq/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/imager/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/imager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/imager/imager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/koboldai/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/koboldai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/koboldai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/leo/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/leo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/leo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/llama2/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/llama2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/llama2/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/openai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/opengpt/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/opengpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/opengpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/perplexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/perplexity/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/phind/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/phind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/phind/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/poe/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/poe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/poe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23689 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/webchatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/webchatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/webchatgpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.121254 python_tgpt-0.6.3/src/python_tgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19666 2024-04-15 09:54:57.000000 python_tgpt-0.6.3/src/python_tgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 09:54:57.000000 python_tgpt-0.6.3/src/python_tgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:54:57.000000 python_tgpt-0.6.3/src/python_tgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 09:54:57.000000 python_tgpt-0.6.3/src/python_tgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-15 09:54:57.000000 python_tgpt-0.6.3/src/python_tgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 09:54:57.000000 python_tgpt-0.6.3/src/python_tgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.121254 python_tgpt-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_blackboxai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_koboldai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_leo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_opengpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_webchatgpt.py
```

### Comparing `python_tgpt-0.6.2/LICENSE` & `python_tgpt-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/PKG-INFO` & `python_tgpt-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.6.2
+Version: 0.6.3
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.2 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.3 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
```

### Comparing `python_tgpt-0.6.2/README.md` & `python_tgpt-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/setup.py` & `python_tgpt-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="python-tgpt",
-    version="0.6.2",
+    version="0.6.3",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Interact with AI without API key",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `python_tgpt-0.6.2/src/pytgpt/__init__.py` & `python_tgpt-0.6.3/src/pytgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/api/__init__.py` & `python_tgpt-0.6.3/src/pytgpt/api/__init__.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/api/v1.py` & `python_tgpt-0.6.3/src/pytgpt/api/v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from fastapi.responses import Response, StreamingResponse, RedirectResponse
 from fastapi.encoders import jsonable_encoder
 from json import dumps
 from pydantic import BaseModel, validator, PositiveInt
 from typing import Union, Any, Generator
 from pytgpt import gpt4free_providers
 from uuid import uuid4
+from .utils import api_exception_handler
 
 # providers
 from pytgpt.leo import LEO
 from pytgpt.opengpt import OPENGPT
 from pytgpt.koboldai import KOBOLDAI
 from pytgpt.phind import PHIND
 from pytgpt.llama2 import LLAMA2
@@ -239,179 +240,150 @@
 
     **Warning** : Not all of *g4f-based* providers are functional.
     """
     return ProvidersModel()
 
 
 @app.post("/chat/nostream", name="no-stream")
+@api_exception_handler
 async def non_stream(payload: UserPayload) -> ProviderResponse:
     """No response streaming.
 
     - `prompt` : User query.
     - `provider` : LLM provider name.
     - `whole` : Return whole response body instead of text only.
     - `max_tokens` : Maximum number of tokens to be generated upon completion.
     - `timeout` : Http request timeout.
     - `proxy` : Http request proxy.
 
     *Ensure `proxy` value is correct otherwise make it `null`*
 
     **NOTE** : Example values are modified for illustration purposes.
     """
-    try:
-        provider_obj: LEO = init_provider(payload)
-        ai_generated_text: str = provider_obj.chat(payload.prompt)
-        return ProviderResponse(
-            provider=payload.provider,
-            text=None if payload.whole else ai_generated_text,
-            body=provider_obj.last_response if payload.whole else None,
-        )
-
-    except Exception as e:
-        raise HTTPException(
-            status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
-            detail=str(e),
-        )
+    provider_obj: LEO = init_provider(payload)
+    ai_generated_text: str = provider_obj.chat(payload.prompt)
+    return ProviderResponse(
+        provider=payload.provider,
+        text=None if payload.whole else ai_generated_text,
+        body=provider_obj.last_response if payload.whole else None,
+    )
 
 
 def generate_streaming_response(payload: UserPayload) -> Generator:
+    provider_obj: LEO = init_provider(payload)
 
-    try:
-        provider_obj: LEO = init_provider(payload)
-
-        for text in provider_obj.chat(payload.prompt, stream=True):
-            response = ProviderResponse(
-                provider=payload.provider,
-                text=None if payload.whole else text,
-                body=provider_obj.last_response if payload.whole else None,
-            )
-            yield dumps(jsonable_encoder(response)) + "\n"
-
-    except Exception as e:
-        raise HTTPException(
-            status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
-            detail=str(e),
+    for text in provider_obj.chat(payload.prompt, stream=True):
+        response = ProviderResponse(
+            provider=payload.provider,
+            text=None if payload.whole else text,
+            body=provider_obj.last_response if payload.whole else None,
         )
+        yield dumps(jsonable_encoder(response)) + "\n"
 
 
 @app.post("/chat/stream", name="stream", response_model=ProviderResponse)
+@api_exception_handler
 async def stream(payload: UserPayload) -> Any:
     """Stream back response as received.
 
     - `prompt` : User query.
     - `provider` : LLM provider name.
     - `whole` : Return whole response body instead of text only.
     - `max_tokens` : Maximum number of tokens to be generated upon completion.
     - `timeout` : Http request timeout.
     - `proxy` : Http request proxy.
 
-    *Ensure `proxy` value is correct otherwise make it `null`*
-
-    **NOTE** : Example values are modified for illustration purposes.
+    **NOTE** :
+       - *Example values are modified for illustration purposes.*
+       - *Ensure `proxy` value is correct otherwise make it `null`*
     """
     return StreamingResponse(
         generate_streaming_response(payload),
         media_type="text/event-stream",
     )
 
 
 @app.post("/image", name="prompt-to-image")
+@api_exception_handler
 async def generate_image(payload: ImagePayload, request: Request) -> ImageResponse:
     """Generate images from prompt
 
     - `prompt` : Image description
     - `amount` : Images to be generated. Maximum of 10.
     - `timeout` : Http request timeout.
     - `proxy` : Http request proxies.
 
-    *Ensure `proxy` value is correct otherwise make it `null`*
+    **NOTE** : *Ensure `proxy` value is correct otherwise make it `null`*
     """
-    try:
-        host = f"{request.url.scheme}://{request.url.netloc}"
-        image_gen_obj = Imager(timeout=payload.timeout, proxies=payload.proxy)
-        image_generator = image_gen_obj.generate(
-            prompt=payload.prompt, amount=payload.amount, stream=True
-        )
-        image_urls = image_gen_obj.save(
-            image_generator,
-            name=uuid4().__str__(),
-            dir=api_static_image_dir,
-            filenames_prefix=f"{host}/static/images/",
-        )
-        return ImageResponse(urls=image_urls)
-
-    except Exception as e:
-        raise HTTPException(
-            status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=str(e)
-        )
+    host = f"{request.url.scheme}://{request.url.netloc}"
+    image_gen_obj = Imager(timeout=payload.timeout, proxies=payload.proxy)
+    image_generator = image_gen_obj.generate(
+        prompt=payload.prompt, amount=payload.amount, stream=True
+    )
+    image_urls = image_gen_obj.save(
+        image_generator,
+        name=uuid4().__str__(),
+        dir=api_static_image_dir,
+        filenames_prefix=f"{host}/static/images/",
+    )
+    return ImageResponse(urls=image_urls)
 
 
 @app.post("/image/bytes", name="prompt-to-image (bytes)")
+@api_exception_handler
 async def generate_image(payload: ImageBytesPayload, request: Request) -> Response:
     """Generate images from prompt and return raw bytes
 
     - `prompt` : Image description
     - `timeout` : Http request timeout.
     - `proxy` : Http request proxies.
 
     **Only one image is generated.**
 
     **NOTE** : *Ensure `proxy` value is correct otherwise make it `null`*
     """
-    try:
-        image_gen_obj = Imager(timeout=payload.timeout, proxies=payload.proxy)
-        image_list = image_gen_obj.generate(prompt=payload.prompt)
-        response = Response(
-            image_list[0],
-            media_type="image/jpeg",
-        )
-        response.headers["Content-Disposition"] = (
-            f"attachment; filename={payload.prompt[:25]+'...' if len(payload.prompt)>25 else payload.prompt}.jpeg"
-        )
-        return response
-
-    except Exception as e:
-        raise HTTPException(
-            status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=str(e)
-        )
+    image_gen_obj = Imager(timeout=payload.timeout, proxies=payload.proxy)
+    image_list = image_gen_obj.generate(prompt=payload.prompt)
+    response = Response(
+        image_list[0],
+        media_type="image/jpeg",
+    )
+    response.headers["Content-Disposition"] = (
+        f"attachment; filename={payload.prompt[:25]+'...' if len(payload.prompt)>25 else payload.prompt}.jpeg"
+    )
+    return response
 
 
 @app.get("/image/bytes", name="prompt-to-image (bytes)")
+@api_exception_handler
 async def redirect_image_generation(
     prompt: str, proxy: Union[str, None] = None, timeout: int = 30
 ):
     """Generate images from prompt and return raw bytes
 
     - `prompt` : Image description
     - `timeout` : Http request timeout.
     - `proxy` : Http request proxies.
 
     **Only one image is generated.**
 
     **NOTE** : *Ensure `proxy` value is correct otherwise make it `null`*
     """
-    try:
-        image_gen_obj = Imager(
-            timeout=timeout, proxies={"https": proxy} if proxy else {}
-        )
-        image_list = image_gen_obj.generate(prompt=prompt)
-        response = Response(
-            image_list[0],
-            media_type="image/jpeg",
-        )
-        response.headers["Content-Disposition"] = (
-            f"attachment; filename={prompt[:25]+'...' if len(prompt)>25 else prompt}.jpeg"
-        )
-        return response
-
-    except Exception as e:
-        raise HTTPException(
-            status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=str(e)
-        )
+    image_gen_obj = Imager(timeout=timeout, proxies={"https": proxy} if proxy else {})
+    image_list = image_gen_obj.generate(prompt=prompt)
+    response = Response(
+        image_list[0],
+        media_type="image/jpeg",
+    )
+    response.headers["Content-Disposition"] = (
+        f"attachment; filename={prompt[:25]+'...' if len(prompt)>25 else prompt}.jpeg"
+    )
+    return response
 
 
 @app.get("/image/bytes/redirect", name="prompt-to-image (bytes - redirect) ")
+@api_exception_handler
 async def redirect_image_generation(prompt: str):
     """Redirect image generation request to [pollinations.ai](https://pollinations.ai)"""
     return RedirectResponse(
         f"https://image.pollinations.ai/prompt/{prompt}",
     )
```

### Comparing `python_tgpt-0.6.2/src/pytgpt/base.py` & `python_tgpt-0.6.3/src/pytgpt/base.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/blackboxai/main.py` & `python_tgpt-0.6.3/src/pytgpt/blackboxai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/console.py` & `python_tgpt-0.6.3/src/pytgpt/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -1033,15 +1033,15 @@
     @busy_bar.run()
     def do_rawdog(self, line):
         """Repeat executing last rawdog's python code"""
         assert self.rawdog, "Session not in rawdog mode. Restart with --rawdog"
         self.default(self.bot.get_message(self.bot.last_response))
 
     @busy_bar.run()
-    def default(self, line, exit_on_error: bool = False):
+    def default(self, line, exit_on_error: bool = False, normal_stdout: bool = False):
         """Chat with LLM"""
         if not bool(line):
             return
         if line.startswith("./"):
             os.system(line[2:])
 
         elif self.rawdog:
@@ -1067,14 +1067,28 @@
                         yield self.bot.chat(line, stream=False)
 
                     return for_non_stream() if self.disable_stream else for_stream()
 
                 busy_bar.start_spinning()
                 generated_response = generate_response()
 
+                if normal_stdout or not self.prettify and not self.disable_stream:
+                    # Resolves : https://github.com/Simatwa/python-tgpt/issues/42 & 43
+                    cached_response: str = ""
+                    if not normal_stdout:
+                        busy_bar.stop_spinning()
+                    for response in generated_response:
+                        offset = len(cached_response)
+                        print(response[offset:], end="")
+                        cached_response = response
+                    if not normal_stdout:
+                        # Interactive prompt
+                        print("")
+                    return
+
                 if self.quiet:
                     busy_bar.stop_spinning()
                     console_ = Console()
                     with Live(
                         console=console_,
                         refresh_per_second=16,
                         vertical_overflow=self.vertical_overflow,
@@ -1756,15 +1770,15 @@
             0 if any([quiet, sys.stdout.isatty() == False]) else busy_bar_index
         )
         bot.code_theme = code_theme
         bot.color = font_color
         bot.prettify = prettify
         bot.vertical_overflow = vertical_overflow
         bot.disable_stream = whole
-        bot.default(prompt, True)
+        bot.default(prompt, True, normal_stdout=(sys.stdout.isatty() == False))
 
 
 class Awesome:
     """Awesome commands"""
 
     @staticmethod
     @click.command(context_settings=this.context_settings)
@@ -2381,14 +2395,42 @@
     def run(port, bind, log_level):
         """Launch FastAPI"""
         import uvicorn
         from pytgpt.api import app
 
         uvicorn.run(app, host=bind, port=port, log_level=log_level)
 
+    @staticmethod
+    @click.command(context_settings=this.context_settings)
+    @click.argument("content", required=True, type=click.Choice(["images", "all"]))
+    @click.option("-y", "--yes", is_flag=True, help="Okay to all confirmation prompts")
+    @click.help_option("-h", "--help")
+    def clear(content: str, yes: bool):
+        """Delete api's static contents"""
+        from pytgpt.utils import api_static_image_dir, api_static_dir
+        from pathlib import Path
+        import shutil
+
+        static_contents_map: dict[str, Path] = {
+            "images": api_static_image_dir,
+            "all": api_static_dir,
+        }
+        content_path: Path = static_contents_map[content]
+        if not yes:
+            yess: bool = click.confirm(
+                f"Are you sure to clear {content} '{content_path.as_posix()}'"
+            )
+            if not yess:
+                return
+        else:
+            pass
+        total_entries = len(os.listdir(content_path))
+        shutil.rmtree(content_path)
+        click.secho(f"{content.title()} cleared ({total_entries})", fg="yellow")
+
 
 def make_commands():
     """Make pytgpt chained commands"""
     # webchatgpt
     # Intergration with WebChatGPT https://github.com/Simatwa/WebChatGPT
     EntryGroup.tgpt2_.add_command(webchatgpt, "webchatgpt")
 
@@ -2417,14 +2459,15 @@
     EntryGroup.awesome.add_command(Awesome.whole)
 
     # Image generator
     EntryGroup.tgpt2_.add_command(ImageGen.generate_image, "imager")
 
     # FastAPI
     EntryGroup.api.add_command(API.run)
+    EntryGroup.api.add_command(API.clear)
 
 
 # @this.handle_exception
 def main(*args):
     """Fireup console programmically"""
     sys.argv += list(args)
     args = sys.argv
```

### Comparing `python_tgpt-0.6.2/src/pytgpt/gemini/main.py` & `python_tgpt-0.6.3/src/pytgpt/gemini/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/gpt4all/main.py` & `python_tgpt-0.6.3/src/pytgpt/gpt4all/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/gpt4free/main.py` & `python_tgpt-0.6.3/src/pytgpt/gpt4free/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/gpt4free/utils.py` & `python_tgpt-0.6.3/src/pytgpt/gpt4free/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/groq/main.py` & `python_tgpt-0.6.3/src/pytgpt/groq/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/imager/imager.py` & `python_tgpt-0.6.3/src/pytgpt/imager/imager.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/koboldai/main.py` & `python_tgpt-0.6.3/src/pytgpt/koboldai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/leo/main.py` & `python_tgpt-0.6.3/src/pytgpt/leo/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/llama2/main.py` & `python_tgpt-0.6.3/src/pytgpt/llama2/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/openai/main.py` & `python_tgpt-0.6.3/src/pytgpt/openai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/opengpt/main.py` & `python_tgpt-0.6.3/src/pytgpt/opengpt/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/perplexity/main.py` & `python_tgpt-0.6.3/src/pytgpt/perplexity/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/phind/main.py` & `python_tgpt-0.6.3/src/pytgpt/phind/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/poe/main.py` & `python_tgpt-0.6.3/src/pytgpt/poe/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/pytgpt/utils.py` & `python_tgpt-0.6.3/src/pytgpt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,23 @@
 import re
 import sys
 import click
 from rich.markdown import Markdown
 from rich.console import Console
 from pathlib import Path
 import os
-import shutil
 
 appdir = appdirs.AppDirs("pytgpt", "Smartwa")
 
 default_path = appdir.user_cache_dir
 
 api_static_dir = Path(default_path) / "api"
 
 api_static_image_dir = api_static_dir / "images"
 
-if api_static_image_dir.exists():
-    # Remove static images
-    shutil.rmtree(api_static_image_dir, ignore_errors=True)
-
 os.makedirs(default_path, exist_ok=True)
 os.makedirs(api_static_dir.as_posix(), exist_ok=True)
 os.makedirs(api_static_image_dir.as_posix(), exist_ok=True)
 
 
 def run_system_command(
     command: str,
```

### Comparing `python_tgpt-0.6.2/src/pytgpt/webchatgpt/main.py` & `python_tgpt-0.6.3/src/pytgpt/webchatgpt/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/src/python_tgpt.egg-info/PKG-INFO` & `python_tgpt-0.6.3/src/python_tgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.6.2
+Version: 0.6.3
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.2 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.3 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
```

### Comparing `python_tgpt-0.6.2/src/python_tgpt.egg-info/SOURCES.txt` & `python_tgpt-0.6.3/src/python_tgpt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/pytgpt/__init__.py
 src/pytgpt/__main__.py
 src/pytgpt/base.py
 src/pytgpt/console.py
 src/pytgpt/utils.py
 src/pytgpt/api/__init__.py
 src/pytgpt/api/__main__.py
+src/pytgpt/api/utils.py
 src/pytgpt/api/v1.py
 src/pytgpt/blackboxai/__init__.py
 src/pytgpt/blackboxai/main.py
 src/pytgpt/gemini/__init__.py
 src/pytgpt/gemini/main.py
 src/pytgpt/gpt4all/__init__.py
 src/pytgpt/gpt4all/main.py
```

### Comparing `python_tgpt-0.6.2/tests/test_api.py` & `python_tgpt-0.6.3/tests/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,12 +100,11 @@
         resp = self.client.get(
             "/v1/image/bytes",
             params={
                 "prompt": "Jay Z performing",
             },
         )
         self.assertEqual(resp.status_code, status.HTTP_200_OK)
-        self.assertIn("https://image.pollinations.ai/", resp.url)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `python_tgpt-0.6.2/tests/test_imager.py` & `python_tgpt-0.6.3/tests/test_imager.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.2/tests/test_utils.py` & `python_tgpt-0.6.3/tests/test_utils.py`

 * *Files identical despite different names*

