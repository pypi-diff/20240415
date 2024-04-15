# Comparing `tmp/sonnia-0.2.0.tar.gz` & `tmp/sonnia-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonnia-0.2.0.tar", last modified: Thu Apr  4 08:04:01 2024, max compression
+gzip compressed data, was "sonnia-0.2.1.tar", last modified: Mon Apr 15 09:30:02 2024, max compression
```

## Comparing `sonnia-0.2.0.tar` & `sonnia-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,118 @@
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-04 08:04:01.355399 sonnia-0.2.0/
--rw-r--r--   0 giulioisac   (502) staff       (20)    35149 2023-05-02 09:08:41.000000 sonnia-0.2.0/LICENSE
--rw-r--r--   0 giulioisac   (502) staff       (20)       41 2024-03-28 09:25:15.000000 sonnia-0.2.0/MANIFEST.in
--rw-r--r--   0 giulioisac   (502) staff       (20)     2131 2024-04-04 08:04:01.355026 sonnia-0.2.0/PKG-INFO
--rw-r--r--   0 giulioisac   (502) staff       (20)     6600 2024-03-28 09:54:11.000000 sonnia-0.2.0/README.md
--rw-r--r--   0 giulioisac   (502) staff       (20)       38 2024-04-04 08:04:01.355467 sonnia-0.2.0/setup.cfg
--rw-r--r--   0 giulioisac   (502) staff       (20)     3224 2024-03-28 09:25:16.000000 sonnia-0.2.0/setup.py
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-04 08:04:01.323565 sonnia-0.2.0/sonnia/
--rw-r--r--   0 giulioisac   (502) staff       (20)        0 2023-05-02 09:08:41.000000 sonnia-0.2.0/sonnia/__init__.py
--rw-r--r--   0 giulioisac   (502) staff       (20)     3884 2024-03-28 09:17:07.000000 sonnia-0.2.0/sonnia/classifiers.py
--rw-r--r--   0 giulioisac   (502) staff       (20)     8511 2024-03-28 09:25:16.000000 sonnia-0.2.0/sonnia/compare_repertoires.py
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-04 08:04:01.353949 sonnia-0.2.0/sonnia/default_models/
--rw-r--r--   0 giulioisac   (502) staff       (20)        0 2024-03-28 09:25:16.000000 sonnia-0.2.0/sonnia/default_models/__init__.py
--rwxr-xr-x   0 giulioisac   (502) staff       (20)    23082 2024-03-28 09:25:16.000000 sonnia-0.2.0/sonnia/evaluate.py
--rwxr-xr-x   0 giulioisac   (502) staff       (20)     9182 2024-03-28 09:25:16.000000 sonnia-0.2.0/sonnia/generate.py
--rwxr-xr-x   0 giulioisac   (502) staff       (20)    24980 2024-03-28 09:25:16.000000 sonnia-0.2.0/sonnia/infer.py
--rw-r--r--   0 giulioisac   (502) staff       (20)    23333 2024-03-28 09:25:16.000000 sonnia-0.2.0/sonnia/plotting.py
--rw-r--r--   0 giulioisac   (502) staff       (20)     7678 2024-03-28 09:25:16.000000 sonnia-0.2.0/sonnia/processing.py
--rw-r--r--   0 giulioisac   (502) staff       (20)    59604 2024-03-28 09:25:16.000000 sonnia-0.2.0/sonnia/sonia.py
--rw-r--r--   0 giulioisac   (502) staff       (20)    24578 2024-03-28 09:25:16.000000 sonnia-0.2.0/sonnia/sonia_paired.py
--rw-r--r--   0 giulioisac   (502) staff       (20)    11380 2024-03-28 09:25:16.000000 sonnia-0.2.0/sonnia/sonnia.py
--rw-r--r--   0 giulioisac   (502) staff       (20)    12868 2024-03-28 09:25:16.000000 sonnia-0.2.0/sonnia/sonnia_paired.py
--rw-r--r--   0 giulioisac   (502) staff       (20)    26010 2024-03-28 09:25:16.000000 sonnia-0.2.0/sonnia/utils.py
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-04 08:04:01.354339 sonnia-0.2.0/sonnia.egg-info/
--rw-r--r--   0 giulioisac   (502) staff       (20)     2131 2024-04-04 08:04:01.000000 sonnia-0.2.0/sonnia.egg-info/PKG-INFO
--rw-r--r--   0 giulioisac   (502) staff       (20)      544 2024-04-04 08:04:01.000000 sonnia-0.2.0/sonnia.egg-info/SOURCES.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)        1 2024-04-04 08:04:01.000000 sonnia-0.2.0/sonnia.egg-info/dependency_links.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)      129 2024-04-04 08:04:01.000000 sonnia-0.2.0/sonnia.egg-info/entry_points.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)        1 2024-01-22 08:31:33.000000 sonnia-0.2.0/sonnia.egg-info/not-zip-safe
--rw-r--r--   0 giulioisac   (502) staff       (20)       52 2024-04-04 08:04:01.000000 sonnia-0.2.0/sonnia.egg-info/requires.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)        7 2024-04-04 08:04:01.000000 sonnia-0.2.0/sonnia.egg-info/top_level.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.143513 sonnia-0.2.1/
+-rw-r--r--   0 giulioisac   (502) staff       (20)    35149 2023-05-02 09:08:41.000000 sonnia-0.2.1/LICENSE
+-rw-r--r--   0 giulioisac   (502) staff       (20)       43 2024-04-15 09:23:26.000000 sonnia-0.2.1/MANIFEST.in
+-rw-r--r--   0 giulioisac   (502) staff       (20)    48681 2024-04-15 09:30:02.143163 sonnia-0.2.1/PKG-INFO
+-rw-r--r--   0 giulioisac   (502) staff       (20)     6600 2024-03-28 09:54:11.000000 sonnia-0.2.1/README.md
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1960 2024-04-15 09:29:42.000000 sonnia-0.2.1/pyproject.toml
+-rw-r--r--   0 giulioisac   (502) staff       (20)       38 2024-04-15 09:30:02.143601 sonnia-0.2.1/setup.cfg
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.130170 sonnia-0.2.1/sonnia/
+-rw-r--r--   0 giulioisac   (502) staff       (20)        0 2023-05-02 09:08:41.000000 sonnia-0.2.1/sonnia/__init__.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)     3884 2024-03-28 09:17:07.000000 sonnia-0.2.1/sonnia/classifiers.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)     8511 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/compare_repertoires.py
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.142055 sonnia-0.2.1/sonnia/default_models/
+-rw-r--r--   0 giulioisac   (502) staff       (20)        0 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/__init__.py
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.106342 sonnia-0.2.1/sonnia/default_models/human_B_heavy/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      255 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     5839 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)    89230 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy/features.tsv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      111 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy/log.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)   483313 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    35291 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.107021 sonnia-0.2.1/sonnia/default_models/human_B_heavy_kappa/
+-rw-r--r--   0 giulioisac   (502) staff       (20)   174156 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_kappa/features.tsv
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.108173 sonnia-0.2.1/sonnia/default_models/human_B_heavy_kappa/heavy_chain/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      255 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_kappa/heavy_chain/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     5839 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_kappa/heavy_chain/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)   483313 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_kappa/heavy_chain/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    35291 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_kappa/heavy_chain/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.109058 sonnia-0.2.1/sonnia/default_models/human_B_heavy_kappa/light_chain/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      144 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_kappa/light_chain/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1179 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_kappa/light_chain/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)    18959 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_kappa/light_chain/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    20986 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_kappa/light_chain/model_params.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)      488 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_kappa/log.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.109552 sonnia-0.2.1/sonnia/default_models/human_B_heavy_lambda/
+-rw-r--r--   0 giulioisac   (502) staff       (20)   173482 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_lambda/features.tsv
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.110619 sonnia-0.2.1/sonnia/default_models/human_B_heavy_lambda/heavy_chain/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      255 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_lambda/heavy_chain/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     5839 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_lambda/heavy_chain/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)   483313 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_lambda/heavy_chain/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    35291 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_lambda/heavy_chain/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.111401 sonnia-0.2.1/sonnia/default_models/human_B_heavy_lambda/light_chain/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      118 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_lambda/light_chain/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1264 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_lambda/light_chain/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)    17632 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_lambda/light_chain/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    23091 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_lambda/light_chain/model_params.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)      308 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_heavy_lambda/log.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.112549 sonnia-0.2.1/sonnia/default_models/human_B_kappa/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      144 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_kappa/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1179 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_kappa/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)    81160 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_kappa/features.tsv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      111 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_kappa/log.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    18959 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_kappa/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    20986 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_kappa/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.113743 sonnia-0.2.1/sonnia/default_models/human_B_lambda/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      118 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_lambda/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1264 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_lambda/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)    84252 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_lambda/features.tsv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      111 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_lambda/log.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    17632 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_lambda/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    23091 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_B_lambda/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.116468 sonnia-0.2.1/sonnia/default_models/human_T_alpha/
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1127 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_alpha/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1901 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_alpha/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)   273848 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_alpha/features.tsv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      111 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_alpha/log.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    75679 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_alpha/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    35883 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_alpha/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.118695 sonnia-0.2.1/sonnia/default_models/human_T_beta/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      283 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     2570 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)   110228 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta/features.tsv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      111 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta/log.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    27384 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    30009 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.119640 sonnia-0.2.1/sonnia/default_models/human_T_beta_alpha/
+-rw-r--r--   0 giulioisac   (502) staff       (20)   369325 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta_alpha/features.tsv
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.121381 sonnia-0.2.1/sonnia/default_models/human_T_beta_alpha/heavy_chain/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      267 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta_alpha/heavy_chain/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     2435 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta_alpha/heavy_chain/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)    30116 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta_alpha/heavy_chain/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    30010 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta_alpha/heavy_chain/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.122469 sonnia-0.2.1/sonnia/default_models/human_T_beta_alpha/light_chain/
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1060 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta_alpha/light_chain/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1901 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta_alpha/light_chain/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)    63471 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta_alpha/light_chain/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    35885 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta_alpha/light_chain/model_params.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1248 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/human_T_beta_alpha/log.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.124530 sonnia-0.2.1/sonnia/default_models/mouse_T_alpha/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      785 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/mouse_T_alpha/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1981 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/mouse_T_alpha/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)   476729 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/mouse_T_alpha/features.tsv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      130 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/mouse_T_alpha/log.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    81928 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/mouse_T_alpha/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    36713 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/mouse_T_alpha/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.125918 sonnia-0.2.1/sonnia/default_models/mouse_T_beta/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      257 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/mouse_T_beta/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      448 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/mouse_T_beta/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)    85621 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/mouse_T_beta/features.tsv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      105 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/mouse_T_beta/log.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    12795 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/mouse_T_beta/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    13475 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/default_models/mouse_T_beta/model_params.txt
+-rwxr-xr-x   0 giulioisac   (502) staff       (20)    23082 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/evaluate.py
+-rwxr-xr-x   0 giulioisac   (502) staff       (20)     9182 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/generate.py
+-rwxr-xr-x   0 giulioisac   (502) staff       (20)    24980 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/infer.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)    23333 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/plotting.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)     7678 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/processing.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)    59604 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/sonia.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)    24578 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/sonia_paired.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)    11380 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/sonnia.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)    12868 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/sonnia_paired.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)    26010 2024-03-28 09:25:16.000000 sonnia-0.2.1/sonnia/utils.py
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:30:02.142364 sonnia-0.2.1/sonnia.egg-info/
+-rw-r--r--   0 giulioisac   (502) staff       (20)    48681 2024-04-15 09:30:02.000000 sonnia-0.2.1/sonnia.egg-info/PKG-INFO
+-rw-r--r--   0 giulioisac   (502) staff       (20)     5070 2024-04-15 09:30:02.000000 sonnia-0.2.1/sonnia.egg-info/SOURCES.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)        1 2024-04-15 09:30:02.000000 sonnia-0.2.1/sonnia.egg-info/dependency_links.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)      129 2024-04-15 09:30:02.000000 sonnia-0.2.1/sonnia.egg-info/entry_points.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)       52 2024-04-15 09:30:02.000000 sonnia-0.2.1/sonnia.egg-info/requires.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)        7 2024-04-15 09:30:02.000000 sonnia-0.2.1/sonnia.egg-info/top_level.txt
```

### Comparing `sonnia-0.2.0/LICENSE` & `sonnia-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sonnia-0.2.0/README.md` & `sonnia-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sonnia-0.2.0/sonnia/classifiers.py` & `sonnia-0.2.1/sonnia/classifiers.py`

 * *Files identical despite different names*

### Comparing `sonnia-0.2.0/sonnia/compare_repertoires.py` & `sonnia-0.2.1/sonnia/compare_repertoires.py`

 * *Files identical despite different names*

### Comparing `sonnia-0.2.0/sonnia/evaluate.py` & `sonnia-0.2.1/sonnia/evaluate.py`

 * *Files identical despite different names*

### Comparing `sonnia-0.2.0/sonnia/generate.py` & `sonnia-0.2.1/sonnia/generate.py`

 * *Files identical despite different names*

### Comparing `sonnia-0.2.0/sonnia/infer.py` & `sonnia-0.2.1/sonnia/infer.py`

 * *Files identical despite different names*

### Comparing `sonnia-0.2.0/sonnia/plotting.py` & `sonnia-0.2.1/sonnia/plotting.py`

 * *Files identical despite different names*

### Comparing `sonnia-0.2.0/sonnia/processing.py` & `sonnia-0.2.1/sonnia/processing.py`

 * *Files identical despite different names*

### Comparing `sonnia-0.2.0/sonnia/sonia.py` & `sonnia-0.2.1/sonnia/sonia.py`

 * *Files identical despite different names*

### Comparing `sonnia-0.2.0/sonnia/sonia_paired.py` & `sonnia-0.2.1/sonnia/sonia_paired.py`

 * *Files identical despite different names*

### Comparing `sonnia-0.2.0/sonnia/sonnia.py` & `sonnia-0.2.1/sonnia/sonnia.py`

 * *Files identical despite different names*

### Comparing `sonnia-0.2.0/sonnia/sonnia_paired.py` & `sonnia-0.2.1/sonnia/sonnia_paired.py`

 * *Files identical despite different names*

### Comparing `sonnia-0.2.0/sonnia/utils.py` & `sonnia-0.2.1/sonnia/utils.py`

 * *Files identical despite different names*

