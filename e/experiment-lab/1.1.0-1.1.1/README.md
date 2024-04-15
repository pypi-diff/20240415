# Comparing `tmp/experiment-lab-1.1.0.tar.gz` & `tmp/experiment_lab-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment-lab-1.1.0.tar", last modified: Fri Apr 12 04:43:36 2024, max compression
+gzip compressed data, was "experiment_lab-1.1.1.tar", last modified: Mon Apr 15 19:35:42 2024, max compression
```

## Comparing `experiment-lab-1.1.0.tar` & `experiment_lab-1.1.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.995277 experiment-lab-1.1.0/
--rw-r--r--   0 rbhagat    (501) staff       (20)     1066 2024-03-01 07:08:11.000000 experiment-lab-1.1.0/LICENCE
--rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/MANIFEST.in
--rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-12 04:43:36.995080 experiment-lab-1.1.0/PKG-INFO
--rw-r--r--   0 rbhagat    (501) staff       (20)     2763 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/README.md
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.986799 experiment-lab-1.1.0/experiment_lab/
--rw-r--r--   0 rbhagat    (501) staff       (20)       75 2024-04-12 04:43:06.000000 experiment-lab-1.1.0/experiment_lab/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.987644 experiment-lab-1.1.0/experiment_lab/common/
--rw-r--r--   0 rbhagat    (501) staff       (20)        0 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/common/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.988016 experiment-lab-1.1.0/experiment_lab/common/networks/
--rw-r--r--   0 rbhagat    (501) staff       (20)      240 2024-03-12 21:19:35.000000 experiment-lab-1.1.0/experiment_lab/common/networks/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1773 2024-03-11 20:50:57.000000 experiment-lab-1.1.0/experiment_lab/common/networks/blocks.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1820 2024-03-12 21:19:35.000000 experiment-lab-1.1.0/experiment_lab/common/networks/mlp.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     6764 2024-04-12 04:43:06.000000 experiment-lab-1.1.0/experiment_lab/common/networks/network.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.988306 experiment-lab-1.1.0/experiment_lab/common/resolvers/
--rw-r--r--   0 rbhagat    (501) staff       (20)      682 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/common/resolvers/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1708 2024-03-12 21:19:35.000000 experiment-lab-1.1.0/experiment_lab/common/resolvers/list_resolvers.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/common/resolvers/object_resolvers.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.988394 experiment-lab-1.1.0/experiment_lab/common/utils/
--rw-r--r--   0 rbhagat    (501) staff       (20)     1548 2024-03-11 19:31:56.000000 experiment-lab-1.1.0/experiment_lab/common/utils/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.988481 experiment-lab-1.1.0/experiment_lab/configs/
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.988726 experiment-lab-1.1.0/experiment_lab/configs/__pycache__/
--rw-r--r--   0 rbhagat    (501) staff       (20)      181 2024-03-02 18:58:05.000000 experiment-lab-1.1.0/experiment_lab/configs/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 rbhagat    (501) staff       (20)       40 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/config.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.989216 experiment-lab-1.1.0/experiment_lab/configs/mc/
--rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/mc/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      750 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/mc/estimate_pi.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.990420 experiment-lab-1.1.0/experiment_lab/configs/rl/
--rw-r--r--   0 rbhagat    (501) staff       (20)      423 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/rl/atari.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      472 2024-04-10 14:31:57.000000 experiment-lab-1.1.0/experiment_lab/configs/rl/cartpole.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)       39 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/rl/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      503 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/rl/crossing.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      534 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/rl/walker.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.991245 experiment-lab-1.1.0/experiment_lab/configs/supervised/
--rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/supervised/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)     2478 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/supervised/fashion_mnist.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.991809 experiment-lab-1.1.0/experiment_lab/core/
--rw-r--r--   0 rbhagat    (501) staff       (20)      265 2024-04-09 22:37:45.000000 experiment-lab-1.1.0/experiment_lab/core/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     5398 2024-04-10 16:31:44.000000 experiment-lab-1.1.0/experiment_lab/core/base_analysis.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-04-10 16:31:44.000000 experiment-lab-1.1.0/experiment_lab/core/base_config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     5645 2024-04-07 19:18:36.000000 experiment-lab-1.1.0/experiment_lab/core/base_experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     2299 2024-04-09 22:28:28.000000 experiment-lab-1.1.0/experiment_lab/core/runner.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.991921 experiment-lab-1.1.0/experiment_lab/experiments/
--rw-r--r--   0 rbhagat    (501) staff       (20)       44 2024-03-04 14:43:06.000000 experiment-lab-1.1.0/experiment_lab/experiments/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.992227 experiment-lab-1.1.0/experiment_lab/experiments/examples/
--rw-r--r--   0 rbhagat    (501) staff       (20)       36 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/experiments/examples/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1767 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/examples/mc_pi_estimate.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/experiments/examples/random_waits.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.992624 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/
--rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.993161 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/
--rw-r--r--   0 rbhagat    (501) staff       (20)      563 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     2328 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/aggregators.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1103 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/post_processors.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1062 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/sample_filters.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1902 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/samplers.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1638 2024-04-03 18:52:52.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     3212 2024-04-03 18:52:52.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      575 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.993779 experiment-lab-1.1.0/experiment_lab/experiments/rl/
--rw-r--r--   0 rbhagat    (501) staff       (20)      255 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/rl/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1421 2024-04-09 22:28:28.000000 experiment-lab-1.1.0/experiment_lab/experiments/rl/analysis.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1852 2024-03-13 20:27:53.000000 experiment-lab-1.1.0/experiment_lab/experiments/rl/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)    10546 2024-04-12 04:43:06.000000 experiment-lab-1.1.0/experiment_lab/experiments/rl/environment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     6267 2024-03-24 16:11:49.000000 experiment-lab-1.1.0/experiment_lab/experiments/rl/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      656 2024-04-09 22:28:28.000000 experiment-lab-1.1.0/experiment_lab/experiments/rl/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.994278 experiment-lab-1.1.0/experiment_lab/experiments/supervised/
--rw-r--r--   0 rbhagat    (501) staff       (20)       63 2024-03-12 21:19:35.000000 experiment-lab-1.1.0/experiment_lab/experiments/supervised/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     3436 2024-03-12 21:19:35.000000 experiment-lab-1.1.0/experiment_lab/experiments/supervised/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     8526 2024-03-13 13:55:28.000000 experiment-lab-1.1.0/experiment_lab/experiments/supervised/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      641 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/experiments/supervised/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.994482 experiment-lab-1.1.0/experiment_lab.egg-info/
--rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-12 04:43:36.000000 experiment-lab-1.1.0/experiment_lab.egg-info/PKG-INFO
--rw-r--r--   0 rbhagat    (501) staff       (20)     2501 2024-04-12 04:43:36.000000 experiment-lab-1.1.0/experiment_lab.egg-info/SOURCES.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)        1 2024-04-12 04:43:36.000000 experiment-lab-1.1.0/experiment_lab.egg-info/dependency_links.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)      237 2024-04-12 04:43:36.000000 experiment-lab-1.1.0/experiment_lab.egg-info/entry_points.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)      223 2024-04-12 04:43:36.000000 experiment-lab-1.1.0/experiment_lab.egg-info/requires.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)       15 2024-04-12 04:43:36.000000 experiment-lab-1.1.0/experiment_lab.egg-info/top_level.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)     1200 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/pyproject.toml
--rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-04-12 04:43:36.995312 experiment-lab-1.1.0/setup.cfg
--rw-r--r--   0 rbhagat    (501) staff       (20)     1030 2024-03-03 02:11:13.000000 experiment-lab-1.1.0/setup.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.332099 experiment_lab-1.1.1/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1066 2024-03-01 07:08:11.000000 experiment_lab-1.1.1/LICENCE
+-rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/MANIFEST.in
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-15 19:35:42.331901 experiment_lab-1.1.1/PKG-INFO
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2763 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/README.md
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.325523 experiment_lab-1.1.1/experiment_lab/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       75 2024-04-15 19:33:48.000000 experiment_lab-1.1.1/experiment_lab/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.326288 experiment_lab-1.1.1/experiment_lab/common/
+-rw-r--r--   0 rbhagat    (501) staff       (20)        0 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/common/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.326776 experiment_lab-1.1.1/experiment_lab/common/networks/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      240 2024-03-12 21:19:35.000000 experiment_lab-1.1.1/experiment_lab/common/networks/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1773 2024-03-11 20:50:57.000000 experiment_lab-1.1.1/experiment_lab/common/networks/blocks.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1820 2024-03-12 21:19:35.000000 experiment_lab-1.1.1/experiment_lab/common/networks/mlp.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     6764 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/common/networks/network.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.327126 experiment_lab-1.1.1/experiment_lab/common/resolvers/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      682 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/common/resolvers/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1708 2024-03-12 21:19:35.000000 experiment_lab-1.1.1/experiment_lab/common/resolvers/list_resolvers.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/common/resolvers/object_resolvers.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.327267 experiment_lab-1.1.1/experiment_lab/common/utils/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1548 2024-03-11 19:31:56.000000 experiment_lab-1.1.1/experiment_lab/common/utils/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.327387 experiment_lab-1.1.1/experiment_lab/configs/
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.327481 experiment_lab-1.1.1/experiment_lab/configs/__pycache__/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      181 2024-03-02 18:58:05.000000 experiment_lab-1.1.1/experiment_lab/configs/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 rbhagat    (501) staff       (20)       40 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/config.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.327674 experiment_lab-1.1.1/experiment_lab/configs/mc/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/mc/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      750 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/mc/estimate_pi.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.328167 experiment_lab-1.1.1/experiment_lab/configs/rl/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      423 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/rl/atari.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      543 2024-04-15 19:33:48.000000 experiment_lab-1.1.1/experiment_lab/configs/rl/cartpole.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)       39 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/rl/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      503 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/rl/crossing.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      534 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/rl/walker.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.328405 experiment_lab-1.1.1/experiment_lab/configs/supervised/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/supervised/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2478 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/supervised/fashion_mnist.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.328988 experiment_lab-1.1.1/experiment_lab/core/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      265 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/core/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     5398 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/core/base_analysis.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/core/base_config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     5645 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/core/base_experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2299 2024-04-15 19:21:43.000000 experiment_lab-1.1.1/experiment_lab/core/runner.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.329074 experiment_lab-1.1.1/experiment_lab/experiments/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       44 2024-03-04 14:43:06.000000 experiment_lab-1.1.1/experiment_lab/experiments/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.329430 experiment_lab-1.1.1/experiment_lab/experiments/examples/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       36 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/experiments/examples/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1767 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/examples/mc_pi_estimate.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/experiments/examples/random_waits.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.329812 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.330294 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      563 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2328 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/aggregators.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1103 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/post_processors.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1062 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/sample_filters.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1902 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/samplers.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1638 2024-04-03 18:52:52.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3212 2024-04-03 18:52:52.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      575 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.330879 experiment_lab-1.1.1/experiment_lab/experiments/rl/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      255 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/rl/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1421 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/experiments/rl/analysis.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1852 2024-03-13 20:27:53.000000 experiment_lab-1.1.1/experiment_lab/experiments/rl/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)    10546 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/experiments/rl/environment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     6423 2024-04-15 19:33:48.000000 experiment_lab-1.1.1/experiment_lab/experiments/rl/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      656 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/experiments/rl/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.331279 experiment_lab-1.1.1/experiment_lab/experiments/supervised/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       63 2024-03-12 21:19:35.000000 experiment_lab-1.1.1/experiment_lab/experiments/supervised/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3436 2024-03-12 21:19:35.000000 experiment_lab-1.1.1/experiment_lab/experiments/supervised/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     8526 2024-03-13 13:55:28.000000 experiment_lab-1.1.1/experiment_lab/experiments/supervised/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      641 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/experiments/supervised/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.331395 experiment_lab-1.1.1/experiment_lab.egg-info/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-15 19:35:42.000000 experiment_lab-1.1.1/experiment_lab.egg-info/PKG-INFO
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2501 2024-04-15 19:35:42.000000 experiment_lab-1.1.1/experiment_lab.egg-info/SOURCES.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)        1 2024-04-15 19:35:42.000000 experiment_lab-1.1.1/experiment_lab.egg-info/dependency_links.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)      237 2024-04-15 19:35:42.000000 experiment_lab-1.1.1/experiment_lab.egg-info/entry_points.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)      223 2024-04-15 19:35:42.000000 experiment_lab-1.1.1/experiment_lab.egg-info/requires.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)       15 2024-04-15 19:35:42.000000 experiment_lab-1.1.1/experiment_lab.egg-info/top_level.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1200 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/pyproject.toml
+-rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-04-15 19:35:42.332129 experiment_lab-1.1.1/setup.cfg
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1030 2024-03-03 02:11:13.000000 experiment_lab-1.1.1/setup.py
```

### Comparing `experiment-lab-1.1.0/LICENCE` & `experiment_lab-1.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/PKG-INFO` & `experiment_lab-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-lab
-Version: 1.1.0
+Version: 1.1.1
 Summary: A suite of flexible experiments of a variety of different tasks.
 Author-email: Rishav Bhagat <rishavbhagat.cs@gmail.com>
 Project-URL: Repository, https://github.com/rishavb123/ExperimentLab
 Keywords: experiment,suite,lab
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `experiment-lab-1.1.0/README.md` & `experiment_lab-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/common/networks/blocks.py` & `experiment_lab-1.1.1/experiment_lab/common/networks/blocks.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/common/networks/mlp.py` & `experiment_lab-1.1.1/experiment_lab/common/networks/mlp.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/common/networks/network.py` & `experiment_lab-1.1.1/experiment_lab/common/networks/network.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/common/resolvers/__init__.py` & `experiment_lab-1.1.1/experiment_lab/common/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/common/resolvers/list_resolvers.py` & `experiment_lab-1.1.1/experiment_lab/common/resolvers/list_resolvers.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/common/utils/__init__.py` & `experiment_lab-1.1.1/experiment_lab/common/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/configs/mc/estimate_pi.yaml` & `experiment_lab-1.1.1/experiment_lab/configs/mc/estimate_pi.yaml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/configs/rl/walker.yaml` & `experiment_lab-1.1.1/experiment_lab/configs/rl/walker.yaml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/configs/supervised/fashion_mnist.yaml` & `experiment_lab-1.1.1/experiment_lab/configs/supervised/fashion_mnist.yaml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/core/base_analysis.py` & `experiment_lab-1.1.1/experiment_lab/core/base_analysis.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/core/base_config.py` & `experiment_lab-1.1.1/experiment_lab/core/base_config.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/core/base_experiment.py` & `experiment_lab-1.1.1/experiment_lab/core/base_experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/core/runner.py` & `experiment_lab-1.1.1/experiment_lab/core/runner.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/examples/mc_pi_estimate.py` & `experiment_lab-1.1.1/experiment_lab/experiments/examples/mc_pi_estimate.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/examples/random_waits.py` & `experiment_lab-1.1.1/experiment_lab/experiments/examples/random_waits.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/__init__.py` & `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/aggregators.py` & `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/aggregators.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/post_processors.py` & `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/post_processors.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/sample_filters.py` & `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/sample_filters.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/samplers.py` & `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/samplers.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/config.py` & `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/config.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/experiment.py` & `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/main.py` & `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/main.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/rl/analysis.py` & `experiment_lab-1.1.1/experiment_lab/experiments/rl/analysis.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/rl/config.py` & `experiment_lab-1.1.1/experiment_lab/experiments/rl/config.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/rl/environment.py` & `experiment_lab-1.1.1/experiment_lab/experiments/rl/environment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/rl/experiment.py` & `experiment_lab-1.1.1/experiment_lab/experiments/rl/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """The rl experiment python file."""
 
 import os
 from typing import Any, List, Type, Dict
+import copy
 import gymnasium as gym
 import hydra
+from omegaconf import OmegaConf
 import torch
 from wandb.integration.sb3 import WandbCallback
 
 from stable_baselines3.common.callbacks import CallbackList
-from stable_baselines3.common.base_class import BaseAlgorithm
 from stable_baselines3.common.policies import BasePolicy
 from stable_baselines3.common.callbacks import BaseCallback
 from stable_baselines3.common.vec_env import VecVideoRecorder
 
 
 from experiment_lab.core.base_experiment import BaseExperiment
 from experiment_lab.experiments.rl.config import RLConfig
@@ -124,22 +125,23 @@
         env.seed(seed)
         env.reset()
 
         # Setup the model
         model = hydra.utils.instantiate(
             {
                 "_target_": self.cfg.model_cls,
+                "policy": self.policy_cls,
+                "policy_kwargs": self.cfg.policy_kwargs,
+                **self.model_kwargs,
             },
             env=env,
-            policy=self.policy_cls,
-            policy_kwargs=self.cfg.policy_kwargs,
             device=self.device,
             tensorboard_log=f"./logs/" if self.cfg.log else None,
             verbose=self.cfg.verbose,
-            **self.model_kwargs,
+            _convert_="partial",
         )
         model.set_random_seed(seed)
         model_save_path = f"{run_output_path}/models/"
 
         # Instantiate the callbacks
         callback_instances = []
         if (
@@ -155,15 +157,20 @@
                     verbose=self.cfg.verbose,
                 )
             )
         for callback_cls, callback_kwargs in zip(
             self.callback_cls_lst, self.callback_kwargs_lst
         ):
             callback_instances.append(
-                callback_cls(**hydra.utils.instantiate(callback_kwargs))
+                hydra.utils.instantiate(
+                    {
+                        "_target_": callback_cls,
+                        **callback_kwargs,
+                    }
+                )
             )
 
         # Run the algorithm
         model.learn(
             total_timesteps=self.cfg.total_time_steps,
             log_interval=self.cfg.log_interval,
             tb_log_name=run_id,
```

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/rl/main.py` & `experiment_lab-1.1.1/experiment_lab/experiments/rl/main.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/supervised/config.py` & `experiment_lab-1.1.1/experiment_lab/experiments/supervised/config.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/supervised/experiment.py` & `experiment_lab-1.1.1/experiment_lab/experiments/supervised/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab/experiments/supervised/main.py` & `experiment_lab-1.1.1/experiment_lab/experiments/supervised/main.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/experiment_lab.egg-info/PKG-INFO` & `experiment_lab-1.1.1/experiment_lab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-lab
-Version: 1.1.0
+Version: 1.1.1
 Summary: A suite of flexible experiments of a variety of different tasks.
 Author-email: Rishav Bhagat <rishavbhagat.cs@gmail.com>
 Project-URL: Repository, https://github.com/rishavb123/ExperimentLab
 Keywords: experiment,suite,lab
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `experiment-lab-1.1.0/experiment_lab.egg-info/SOURCES.txt` & `experiment_lab-1.1.1/experiment_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/pyproject.toml` & `experiment_lab-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.1.0/setup.py` & `experiment_lab-1.1.1/setup.py`

 * *Files identical despite different names*

