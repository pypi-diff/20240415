# Comparing `tmp/mpcrl-1.2.0rc4.tar.gz` & `tmp/mpcrl-1.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcrl-1.2.0rc4.tar", last modified: Fri Apr  5 20:49:47 2024, max compression
+gzip compressed data, was "mpcrl-1.2.1rc1.tar", last modified: Mon Apr 15 15:20:50 2024, max compression
```

## Comparing `mpcrl-1.2.0rc4.tar` & `mpcrl-1.2.1rc1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.474789 mpcrl-1.2.0rc4/
--rw-rw-rw-   0        0        0     1093 2022-11-28 16:28:05.000000 mpcrl-1.2.0rc4/LICENSE
--rw-rw-rw-   0        0        0     6181 2024-04-05 20:49:47.473775 mpcrl-1.2.0rc4/PKG-INFO
--rw-rw-rw-   0        0        0     4935 2023-12-29 16:34:56.000000 mpcrl-1.2.0rc4/README.md
--rw-rw-rw-   0        0        0     2198 2024-03-20 18:16:17.000000 mpcrl-1.2.0rc4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 20:49:47.474789 mpcrl-1.2.0rc4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.413842 mpcrl-1.2.0rc4/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.423898 mpcrl-1.2.0rc4/src/mpcrl/
--rw-rw-rw-   0        0        0     1289 2024-03-22 14:09:50.000000 mpcrl-1.2.0rc4/src/mpcrl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.433929 mpcrl-1.2.0rc4/src/mpcrl/agents/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.438937 mpcrl-1.2.0rc4/src/mpcrl/agents/common/
--rw-rw-rw-   0        0        0    24076 2024-03-23 23:52:56.000000 mpcrl-1.2.0rc4/src/mpcrl/agents/common/agent.py
--rw-rw-rw-   0        0        0     3389 2024-03-23 23:36:33.000000 mpcrl-1.2.0rc4/src/mpcrl/agents/common/globopt_learning_agent.py
--rw-rw-rw-   0        0        0    13551 2024-03-23 23:58:18.000000 mpcrl-1.2.0rc4/src/mpcrl/agents/common/learning_agent.py
--rw-rw-rw-   0        0        0     1749 2024-02-02 22:17:54.000000 mpcrl-1.2.0rc4/src/mpcrl/agents/common/offpolicy_rl_agent copy.py
--rw-rw-rw-   0        0        0     1749 2024-02-02 22:17:54.000000 mpcrl-1.2.0rc4/src/mpcrl/agents/common/rl_learning_agent.py
--rw-rw-rw-   0        0        0    20477 2024-03-20 15:43:51.000000 mpcrl-1.2.0rc4/src/mpcrl/agents/lstd_dpg.py
--rw-rw-rw-   0        0        0    15173 2024-03-20 15:44:06.000000 mpcrl-1.2.0rc4/src/mpcrl/agents/lstd_q_learning.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.443957 mpcrl-1.2.0rc4/src/mpcrl/core/
--rw-rw-rw-   0        0        0        0 2023-10-26 16:39:29.000000 mpcrl-1.2.0rc4/src/mpcrl/core/__init__.py
--rw-rw-rw-   0        0        0     9816 2024-02-03 22:29:54.000000 mpcrl-1.2.0rc4/src/mpcrl/core/callbacks.py
--rw-rw-rw-   0        0        0     1609 2023-01-07 11:39:22.000000 mpcrl-1.2.0rc4/src/mpcrl/core/errors.py
--rw-rw-rw-   0        0        0     3294 2023-12-29 16:11:51.000000 mpcrl-1.2.0rc4/src/mpcrl/core/experience.py
--rw-rw-rw-   0        0        0    12631 2023-12-29 16:11:51.000000 mpcrl-1.2.0rc4/src/mpcrl/core/exploration.py
--rw-rw-rw-   0        0        0    12085 2023-10-26 16:39:29.000000 mpcrl-1.2.0rc4/src/mpcrl/core/parameters.py
--rw-rw-rw-   0        0        0     7143 2023-10-26 16:39:17.000000 mpcrl-1.2.0rc4/src/mpcrl/core/schedulers.py
--rw-rw-rw-   0        0        0     2537 2023-10-26 16:39:29.000000 mpcrl-1.2.0rc4/src/mpcrl/core/update.py
--rw-rw-rw-   0        0        0     5167 2024-03-22 13:40:45.000000 mpcrl-1.2.0rc4/src/mpcrl/core/warmstart.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.443957 mpcrl-1.2.0rc4/src/mpcrl/optim/
--rw-rw-rw-   0        0        0      482 2024-02-02 21:55:26.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/__init__.py
--rw-rw-rw-   0        0        0     7193 2023-10-26 16:39:29.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/adam.py
--rw-rw-rw-   0        0        0     2600 2023-12-29 18:05:40.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/base_optimizer.py
--rw-rw-rw-   0        0        0     6668 2023-12-29 18:04:08.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/gradient_based_optimizer.py
--rw-rw-rw-   0        0        0     5624 2023-10-26 16:39:29.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/gradient_descent.py
--rw-rw-rw-   0        0        0     2429 2023-12-30 18:29:00.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/gradient_free_optimizer.py
--rw-rw-rw-   0        0        0     6712 2023-10-26 16:39:29.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/newton_method.py
--rw-rw-rw-   0        0        0     6532 2023-10-26 16:39:29.000000 mpcrl-1.2.0rc4/src/mpcrl/optim/rmsprop.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.459354 mpcrl-1.2.0rc4/src/mpcrl/util/
--rw-rw-rw-   0        0        0     2785 2023-08-28 20:00:11.000000 mpcrl-1.2.0rc4/src/mpcrl/util/control.py
--rw-rw-rw-   0        0        0      800 2023-09-21 13:43:47.000000 mpcrl-1.2.0rc4/src/mpcrl/util/iters.py
--rw-rw-rw-   0        0        0     4855 2023-10-26 16:35:58.000000 mpcrl-1.2.0rc4/src/mpcrl/util/math.py
--rw-rw-rw-   0        0        0      933 2023-09-21 13:43:47.000000 mpcrl-1.2.0rc4/src/mpcrl/util/named.py
--rw-rw-rw-   0        0        0      638 2023-12-29 16:11:53.000000 mpcrl-1.2.0rc4/src/mpcrl/util/seeding.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.418847 mpcrl-1.2.0rc4/src/mpcrl/wrappers/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.462350 mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/
--rw-rw-rw-   0        0        0      180 2023-10-26 16:37:23.000000 mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/__init__.py
--rw-rw-rw-   0        0        0     8402 2024-02-02 21:42:27.000000 mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/log.py
--rw-rw-rw-   0        0        0     1261 2024-02-02 21:42:27.000000 mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/record_updates.py
--rw-rw-rw-   0        0        0     4998 2024-02-02 21:42:27.000000 mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.464350 mpcrl-1.2.0rc4/src/mpcrl/wrappers/envs/
--rw-rw-rw-   0        0        0      137 2023-10-26 16:37:23.000000 mpcrl-1.2.0rc4/src/mpcrl/wrappers/envs/__init__.py
--rw-rw-rw-   0        0        0     4446 2024-03-20 13:12:09.000000 mpcrl-1.2.0rc4/src/mpcrl/wrappers/envs/monitor_episodes.py
--rw-rw-rw-   0        0        0     4939 2023-09-21 13:43:47.000000 mpcrl-1.2.0rc4/src/mpcrl/wrappers/envs/monitor_infos.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.472754 mpcrl-1.2.0rc4/src/mpcrl.egg-info/
--rw-rw-rw-   0        0        0     6181 2024-04-05 20:49:47.000000 mpcrl-1.2.0rc4/src/mpcrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1543 2024-04-05 20:49:47.000000 mpcrl-1.2.0rc4/src/mpcrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 20:49:47.000000 mpcrl-1.2.0rc4/src/mpcrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-05 20:49:47.000000 mpcrl-1.2.0rc4/src/mpcrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-05 20:49:47.000000 mpcrl-1.2.0rc4/src/mpcrl.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 20:49:47.470224 mpcrl-1.2.0rc4/tests/
--rw-rw-rw-   0        0        0    15889 2023-12-29 16:11:53.000000 mpcrl-1.2.0rc4/tests/test_agent.py
--rw-rw-rw-   0        0        0    22905 2023-10-26 16:39:25.000000 mpcrl-1.2.0rc4/tests/test_core.py
--rw-rw-rw-   0        0        0    11156 2024-02-09 18:59:51.000000 mpcrl-1.2.0rc4/tests/test_examples.py
--rw-rw-rw-   0        0        0    18686 2023-12-29 18:06:31.000000 mpcrl-1.2.0rc4/tests/test_optim.py
--rw-rw-rw-   0        0        0     5040 2023-12-29 16:11:53.000000 mpcrl-1.2.0rc4/tests/test_util.py
--rw-rw-rw-   0        0        0    14705 2023-12-29 16:11:49.000000 mpcrl-1.2.0rc4/tests/test_wrappers.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.393318 mpcrl-1.2.1rc1/
+-rw-rw-rw-   0        0        0     1093 2022-11-28 16:28:05.000000 mpcrl-1.2.1rc1/LICENSE
+-rw-rw-rw-   0        0        0     6178 2024-04-15 15:20:50.388285 mpcrl-1.2.1rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     4935 2024-04-12 22:21:05.000000 mpcrl-1.2.1rc1/README.md
+-rw-rw-rw-   0        0        0     2195 2024-04-11 13:47:55.000000 mpcrl-1.2.1rc1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 15:20:50.394284 mpcrl-1.2.1rc1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.092159 mpcrl-1.2.1rc1/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.131464 mpcrl-1.2.1rc1/src/mpcrl/
+-rw-rw-rw-   0        0        0     1289 2024-04-15 14:55:11.000000 mpcrl-1.2.1rc1/src/mpcrl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.164863 mpcrl-1.2.1rc1/src/mpcrl/agents/
+drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.185846 mpcrl-1.2.1rc1/src/mpcrl/agents/common/
+-rw-rw-rw-   0        0        0    27020 2024-04-15 15:18:33.000000 mpcrl-1.2.1rc1/src/mpcrl/agents/common/agent.py
+-rw-rw-rw-   0        0        0     3707 2024-04-11 13:45:23.000000 mpcrl-1.2.1rc1/src/mpcrl/agents/common/globopt_learning_agent.py
+-rw-rw-rw-   0        0        0    14240 2024-04-15 14:42:04.000000 mpcrl-1.2.1rc1/src/mpcrl/agents/common/learning_agent.py
+-rw-rw-rw-   0        0        0     1749 2024-04-11 13:45:25.000000 mpcrl-1.2.1rc1/src/mpcrl/agents/common/rl_learning_agent.py
+-rw-rw-rw-   0        0        0    23054 2024-04-13 20:46:44.000000 mpcrl-1.2.1rc1/src/mpcrl/agents/lstd_dpg.py
+-rw-rw-rw-   0        0        0    15340 2024-04-13 19:50:03.000000 mpcrl-1.2.1rc1/src/mpcrl/agents/lstd_q_learning.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.231047 mpcrl-1.2.1rc1/src/mpcrl/core/
+-rw-rw-rw-   0        0        0        0 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc1/src/mpcrl/core/__init__.py
+-rw-rw-rw-   0        0        0     9809 2024-04-15 11:58:24.000000 mpcrl-1.2.1rc1/src/mpcrl/core/callbacks.py
+-rw-rw-rw-   0        0        0     1609 2023-01-07 11:39:22.000000 mpcrl-1.2.1rc1/src/mpcrl/core/errors.py
+-rw-rw-rw-   0        0        0     3461 2024-04-12 22:21:05.000000 mpcrl-1.2.1rc1/src/mpcrl/core/experience.py
+-rw-rw-rw-   0        0        0    16018 2024-04-12 22:21:05.000000 mpcrl-1.2.1rc1/src/mpcrl/core/exploration.py
+-rw-rw-rw-   0        0        0    12085 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc1/src/mpcrl/core/parameters.py
+-rw-rw-rw-   0        0        0     7143 2023-10-26 16:39:17.000000 mpcrl-1.2.1rc1/src/mpcrl/core/schedulers.py
+-rw-rw-rw-   0        0        0     2537 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc1/src/mpcrl/core/update.py
+-rw-rw-rw-   0        0        0     4713 2024-04-11 13:48:00.000000 mpcrl-1.2.1rc1/src/mpcrl/core/warmstart.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.276213 mpcrl-1.2.1rc1/src/mpcrl/optim/
+-rw-rw-rw-   0        0        0      482 2024-04-11 13:45:23.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/__init__.py
+-rw-rw-rw-   0        0        0     7193 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/adam.py
+-rw-rw-rw-   0        0        0     2600 2024-04-11 13:45:13.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/base_optimizer.py
+-rw-rw-rw-   0        0        0     6668 2024-04-11 13:45:13.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/gradient_based_optimizer.py
+-rw-rw-rw-   0        0        0     5624 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/gradient_descent.py
+-rw-rw-rw-   0        0        0     2429 2024-04-11 13:45:15.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/gradient_free_optimizer.py
+-rw-rw-rw-   0        0        0     6712 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/newton_method.py
+-rw-rw-rw-   0        0        0     6532 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/rmsprop.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.299216 mpcrl-1.2.1rc1/src/mpcrl/util/
+-rw-rw-rw-   0        0        0     2785 2023-08-28 20:00:11.000000 mpcrl-1.2.1rc1/src/mpcrl/util/control.py
+-rw-rw-rw-   0        0        0      800 2023-09-21 13:43:47.000000 mpcrl-1.2.1rc1/src/mpcrl/util/iters.py
+-rw-rw-rw-   0        0        0     4855 2023-10-26 16:35:58.000000 mpcrl-1.2.1rc1/src/mpcrl/util/math.py
+-rw-rw-rw-   0        0        0      933 2023-09-21 13:43:47.000000 mpcrl-1.2.1rc1/src/mpcrl/util/named.py
+-rw-rw-rw-   0        0        0      638 2023-12-29 16:11:53.000000 mpcrl-1.2.1rc1/src/mpcrl/util/seeding.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.113464 mpcrl-1.2.1rc1/src/mpcrl/wrappers/
+drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.326800 mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/
+-rw-rw-rw-   0        0        0      224 2024-04-15 13:57:59.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/__init__.py
+-rw-rw-rw-   0        0        0     4615 2024-04-15 14:38:03.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/evaluate.py
+-rw-rw-rw-   0        0        0     8402 2024-04-11 13:45:23.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/log.py
+-rw-rw-rw-   0        0        0     1261 2024-04-11 13:45:23.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/record_updates.py
+-rw-rw-rw-   0        0        0     4832 2024-04-15 12:11:27.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.343797 mpcrl-1.2.1rc1/src/mpcrl/wrappers/envs/
+-rw-rw-rw-   0        0        0      137 2023-10-26 16:37:23.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/envs/__init__.py
+-rw-rw-rw-   0        0        0     4446 2024-04-11 13:47:27.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/envs/monitor_episodes.py
+-rw-rw-rw-   0        0        0     4939 2023-09-21 13:43:47.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/envs/monitor_infos.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.382282 mpcrl-1.2.1rc1/src/mpcrl.egg-info/
+-rw-rw-rw-   0        0        0     6178 2024-04-15 15:20:50.000000 mpcrl-1.2.1rc1/src/mpcrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1530 2024-04-15 15:20:50.000000 mpcrl-1.2.1rc1/src/mpcrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 15:20:50.000000 mpcrl-1.2.1rc1/src/mpcrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-04-15 15:20:50.000000 mpcrl-1.2.1rc1/src/mpcrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-15 15:20:50.000000 mpcrl-1.2.1rc1/src/mpcrl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.377290 mpcrl-1.2.1rc1/tests/
+-rw-rw-rw-   0        0        0    16493 2024-04-12 22:21:05.000000 mpcrl-1.2.1rc1/tests/test_agent.py
+-rw-rw-rw-   0        0        0    24223 2024-04-12 22:21:05.000000 mpcrl-1.2.1rc1/tests/test_core.py
+-rw-rw-rw-   0        0        0    12018 2024-04-15 15:18:20.000000 mpcrl-1.2.1rc1/tests/test_examples.py
+-rw-rw-rw-   0        0        0    18686 2024-04-11 13:45:13.000000 mpcrl-1.2.1rc1/tests/test_optim.py
+-rw-rw-rw-   0        0        0     5040 2023-12-29 16:11:53.000000 mpcrl-1.2.1rc1/tests/test_util.py
+-rw-rw-rw-   0        0        0    16530 2024-04-15 14:49:52.000000 mpcrl-1.2.1rc1/tests/test_wrappers.py
```

### Comparing `mpcrl-1.2.0rc4/LICENSE` & `mpcrl-1.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/PKG-INFO` & `mpcrl-1.2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcrl
-Version: 1.2.0rc4
+Version: 1.2.1rc1
 Summary: Reinforcement Learning with Model Predictive Control
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/mpc-reinforcement-learning
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues
 Keywords: reinforcement-learning,model-predictive-control,optimization,casadi
 Classifier: Programming Language :: Python
@@ -18,15 +18,15 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions>=4.5.0
 Requires-Dist: numba>=0.57.1
-Requires-Dist: csnlp>=1.5.10rc3
+Requires-Dist: csnlp>=1.5.10
 Requires-Dist: scipy>=1.11.0
 Requires-Dist: gymnasium>=0.28.1
 
 # Reinforcement Learning with Model Predictive Control
 
 **mpcrl** is a library for training model-based Reinforcement Learning (RL) agents with Model Predictive Control (MPC) as function approximation. This framework, also known as MPC-based RL, was first proposed in [[1]](#1) and has so far been shown effective in various applications and with different learning algorithms, e.g., [[2](#2),[3](#3)].
```

### Comparing `mpcrl-1.2.0rc4/README.md` & `mpcrl-1.2.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/pyproject.toml` & `mpcrl-1.2.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "typing_extensions >= 4.5.0",
     "numba >= 0.57.1",
-    "csnlp >= 1.5.10rc3",
+    "csnlp >= 1.5.10",
     "scipy >= 1.11.0",
     "gymnasium >= 0.28.1",
 ]
 keywords = [
     "reinforcement-learning",
     "model-predictive-control",
     "optimization",
```

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/__init__.py` & `mpcrl-1.2.1rc1/src/mpcrl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.0rc4"
+__version__ = "1.2.1rc1"
 
 __all__ = [
     "Agent",
     "ExperienceReplay",
     "GlobOptLearningAgent",
     "LearnableParameter",
     "LearnableParametersDict",
```

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/agents/common/agent.py` & `mpcrl-1.2.1rc1/src/mpcrl/agents/common/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import numpy as np
 import numpy.typing as npt
 from csnlp import Solution, wrappers
 from csnlp.core.cache import invalidate_caches_of
 from csnlp.util.io import SupportsDeepcopyAndPickle
 from csnlp.wrappers import Mpc
 from gymnasium import Env
+from gymnasium.spaces import Box
 from typing_extensions import TypeAlias
 
 from ...core.callbacks import AgentCallbackMixin
 from ...core.exploration import ExplorationStrategy, NoExploration
 from ...core.warmstart import WarmStartStrategy
 from ...util.named import Named
 from ...util.seeding import RngType, mk_seed
@@ -44,14 +45,15 @@
 
     def __init__(
         self,
         mpc: Mpc[SymType],
         fixed_parameters: Union[
             None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]
         ] = None,
+        exploration: Optional[ExplorationStrategy] = None,
         warmstart: Union[
             Literal["last", "last-successful"], WarmStartStrategy
         ] = "last-successful",
         use_last_action_on_fail: bool = False,
         remove_bounds_on_initial_action: bool = False,
         name: Optional[str] = None,
     ) -> None:
@@ -68,19 +70,22 @@
             names are already in use in the mpc. These names are under the attributes
             `perturbation_parameter`, `action_parameter` and `action_constraint`.
         fixed_parameters : dict[str, array_like] or collection of, optional
             A dict (or collection of dict, in case of `csnlp.MultistartNlp`) whose keys
             are the names of the MPC parameters and the values are their corresponding
             values. Use this to specify fixed parameters, that is, non-learnable. If
             `None`, then no fixed parameter is assumed.
+        exploration : ExplorationStrategy, optional
+            Exploration strategy for inducing exploration in the MPC policy. By default
+            `None`, in which case `NoExploration` is used.
         warmstart: "last" or "last-successful" or WarmStartStrategy, optional
             The warmstart strategy for the MPC's NLP. If `last-successful`, the last
             successful solution is used to warm start the solver for the next iteration.
             If `last`, the last solution is used, regardless of success or failure.
-            Furthermoer, a `WarmStartStrategy` object can be passed to specify a
+            Furthermore, a `WarmStartStrategy` object can be passed to specify a
             strategy for generating multiple warmstart points for the NLP. This is
             useful to generate multiple initial conditions for very non-convex problems.
             Can only be used with an MPC that has an underlying multistart NLP problem
             (see `csnlp.MultistartNlp`).
         use_last_action_on_fail : bool, optional
             In case the MPC solver fails
              * if `False`, the action from the last solver's iteration is returned
@@ -98,25 +103,44 @@
         name : str, optional
             Name of the agent. If `None`, one is automatically created from a counter of
             the class' instancies.
 
         Raises
         ------
         ValueError
-            Raises if the given mpc has no control action as optimization variable; or
-            if the required parameter and constraint names are already specified in the
-            mpc.
+            Raises if
+             * the given mpc has no control action as optimization variable
+             * the reserved parameter and constraint names are already in use
+             * a multistart MPC is given, but the warmstart strategy asks for an
+               incompatible number of starting points to be generated
+             * a warmstart strategy is given, but the MPC does not have an underlying
+               multistart NLP problem, so it cannot handle multiple starting points.
         """
+        if isinstance(warmstart, str):
+            warmstart = WarmStartStrategy(warmstart)
+        ws_points = warmstart.n_points
+        if mpc.is_multi and ws_points != 0 and mpc.nlp.starts - ws_points not in (0, 1):
+            raise ValueError(
+                "A multistart MPC was given with {mpc.nlp.starts} multistarts, but the "
+                f"given warmstart strategy asks for {ws_points} starting points. "
+                "Expected either 0 warmstart points (i.e., it is disabled), or the same"
+                " number as MPC's multistarts, or at most one less."
+            )
+        elif not mpc.is_multi and ws_points > 0:
+            raise ValueError(
+                "Got a warmstart strategy with more than 0 starting points, but the "
+                "given does not have an underlying multistart NLP problem."
+            )
         Named.__init__(self, name)
         SupportsDeepcopyAndPickle.__init__(self)
         AgentCallbackMixin.__init__(self)
         self._fixed_pars = fixed_parameters
-        self._exploration: ExplorationStrategy = NoExploration()
-        if isinstance(warmstart, str):
-            warmstart = WarmStartStrategy(warmstart)
+        if exploration is None:
+            exploration = NoExploration()
+        self._exploration = exploration
         self._warmstart = warmstart
         self._last_action_on_fail = use_last_action_on_fail
         self._last_solution: Optional[Solution[SymType]] = None
         self._last_action: Optional[cs.DM] = None
         self._V, self._Q = self._setup_V_and_Q(mpc, remove_bounds_on_initial_action)
         self._post_setup_V_and_Q()
 
@@ -159,16 +183,15 @@
         return self._warmstart
 
     def reset(self, seed: RngType = None) -> None:
         """Resets the agent's internal variables and exploration's RNG."""
         self._last_solution = None
         self._last_action = None
         self.warmstart.reset(seed)
-        if hasattr(self.exploration, "reset"):
-            self.exploration.reset(seed)
+        self.exploration.reset(seed)
 
     def solve_mpc(
         self,
         mpc: Mpc[SymType],
         state: Union[npt.ArrayLike, dict[str, npt.ArrayLike]],
         action: Union[None, npt.ArrayLike, dict[str, npt.ArrayLike]] = None,
         perturbation: Optional[npt.ArrayLike] = None,
@@ -187,22 +210,23 @@
             A 1D array representing the value of all states of the MPC, concatenated.
             Otherwise, a dict whose keys are the names of each state, and values are
             their numerical values.
         action : array_like or dict[str, array_like], optional
             Same for `state`, for the action. Only valid if evaluating the action value
             function `Q(s,a)`. For this reason, it can be `None` for `V(s)`.
         perturbation : array_like, optional
-            The cost perturbation used to induce exploration in `V(s)`. Can be `None`
-            for `Q(s,a)`.
+            The gradient-based cost perturbation used to induce exploration in `V(s)`.
+            Should be `None` for `Q(s,a)`, or in case of other types of exploration.
         vals0 : dict[str, array_like] or iterable of, optional
             A dict (or an iterable of dict, in case of `csnlp.MultistartNlp`), whose
             keys are the names of the MPC variables, and values are the numerical
             initial values of each variable. Use this to warm-start the MPC. If `None`,
             and a previous solution (possibly, successful) is available, the MPC solver
-            is automatically warm-started.
+            is automatically warm-started. If an iterable is passed instead, the
+            warm-starting strategy is bypassed.
         store_solution : bool, optional
             By default, the mpc solution is stored accordingly to the `warmstart`
             strategy. If set to `False`, this flag allows to disable the behaviour for
             this particular solution.
 
         Returns
         -------
@@ -245,35 +269,38 @@
         elif isinstance(pars, dict):
             pars.update(additional_pars)
         else:  # iterable of dict
             pars = _update_dicts(pars, additional_pars)
         if vals0 is None and self._last_solution is not None:
             vals0 = self._last_solution.vals
 
-        # if available, use the warmstart strategy to generate multiple initial
-        # warm-start points for the NLP - remember to include `vals0` among these
-        if mpc.is_multi and self._warmstart.can_generate:
-            starts = mpc.nlp.starts - 1
-            n = starts // 2
-            vals0_iter = self._warmstart.generate(n, starts - n, vals0)
-            vals0 = chain((vals0,), vals0_iter)
+        # use the warmstart strategy to generate multiple initial points for the NLP if
+        # the NLP supports multi and `vals0` is not already an iterable of dict
+        if mpc.is_multi and (vals0 is None or isinstance(vals0, dict)):
+            more_vals0s = self._warmstart.generate(vals0)
+            if mpc.nlp.starts > self._warmstart.n_points:
+                # the difference between these two has been checked to be at most one,
+                # meaning we can include `vals0` itself
+                more_vals0s = chain((vals0,), more_vals0s)
+            vals0 = more_vals0s
 
         # solve and store solution
         sol = mpc(pars, vals0)
         if store_solution and (self._warmstart.store_always or sol.success):
             self._last_solution = sol
         return sol
 
     def state_value(
         self,
         state: Union[npt.ArrayLike, dict[str, npt.ArrayLike]],
         deterministic: bool = False,
         vals0: Union[
             None, dict[str, npt.ArrayLike], Iterable[dict[str, npt.ArrayLike]]
         ] = None,
+        action_space: Optional[Box] = None,
         **kwargs,
     ) -> tuple[cs.DM, Solution[SymType]]:
         """Computes the state value function `V(s)` approximated by the MPC.
 
         Parameters
         ----------
         state : array_like or dict[str, array_like]
@@ -286,38 +313,55 @@
             performed. By default, `deterministic=False`.
         vals0 : dict[str, array_like] or iterable of, optional
             A dict (or an iterable of dict, in case of `csnlp.MultistartNlp`), whose
             keys are the names of the MPC variables, and values are the numerical
             initial values of each variable. Use this to warm-start the MPC. If `None`,
             and a previous solution (possibly, successful) is available, the MPC solver
             is automatically warm-started.
+        action_space : gymnasium.spaces.Box, optional
+            The action space of the environment. If not `None`, it is used in case an
+            additive exploration perturbation is summed to the action in order to clip
+            it back into the action space.
 
         Returns
         -------
         casadi.DM
-            The first optimal action according to the solution of `V(s)`.
+            The first optimal action according to the solution of `V(s)`, possibly
+            perturbed by exploration noise
         Solution
             The solution of the MPC approximating `V(s)` at the given state.
         """
-        if deterministic or not self._exploration.can_explore():
+        V = self._V
+        exploration = self._exploration
+        exploration_mode = self._exploration.mode
+        na = V.na
+        if deterministic or exploration_mode is None or not exploration.can_explore():
             pert = None
         else:
-            pert = self._exploration.perturbation(
-                self.cost_perturbation_method,
-                size=self.V.parameters[self.cost_perturbation_parameter].shape,
-            )
-        sol = self.solve_mpc(self._V, state, perturbation=pert, vals0=vals0, **kwargs)
-        first_action = cs.vertcat(*(sol.vals[u][:, 0] for u in self._V.actions.keys()))
+            pert = exploration.perturbation(self.cost_perturbation_method, size=(na, 1))
+
+        grad_pert = pert if exploration_mode == "gradient-based" else None
+        sol = self.solve_mpc(V, state, perturbation=grad_pert, vals0=vals0, **kwargs)
+        action_opt = cs.vertcat(*(sol.vals[u][:, 0] for u in V.actions.keys()))
 
         if sol.success:
-            self._last_action = first_action
+            self._last_action = action_opt
         elif self._last_action_on_fail and self._last_action is not None:
-            first_action = self._last_action
+            action_opt = self._last_action
 
-        return first_action, sol
+        if pert is not None and exploration_mode == "additive":
+            action_opt_noisy = action_opt + pert
+            if action_space is not None:
+                lb = action_space.low.reshape(na, 1)
+                ub = action_space.high.reshape(na, 1)
+                action_opt_noisy = np.clip(action_opt_noisy, lb, ub)
+                # if np.equal(action_opt_noisy, action_opt).all():
+                #     action_opt_noisy = np.clip(action_opt - pert, lb, ub)
+            action_opt = action_opt_noisy
+        return action_opt, sol
 
     def action_value(
         self,
         state: Union[npt.ArrayLike, dict[str, npt.ArrayLike]],
         action: Union[npt.ArrayLike, dict[str, npt.ArrayLike]],
         vals0: Union[
             None, dict[str, npt.ArrayLike], Iterable[dict[str, npt.ArrayLike]]
@@ -427,31 +471,33 @@
         if na <= 0:
             raise ValueError(f"Expected Mpc with na>0; got na={na} instead.")
 
         # create V and Q function approximations
         V, Q = mpc, mpc.copy()
         V.unwrapped.name += "_V"
         Q.unwrapped.name += "_Q"
-        a0 = Q.nlp.parameter(self.init_action_parameter, (na, 1))
-        perturbation = V.nlp.parameter(self.cost_perturbation_parameter, (na, 1))
 
+        # for Q, add the additional constraint on the initial action to be equal to a0,
+        # and remove the now useless upper/lower bounds on the initial action
+        a0 = Q.nlp.parameter(self.init_action_parameter, (na, 1))
         u0 = cs.vcat(mpc.first_actions.values())
-        f = V.nlp.f
-        if mpc.is_wrapped(wrappers.NlpScaling):
-            f = mpc.scale(f)
-
-        V.nlp.minimize(f + cs.dot(perturbation, u0))
         Q.nlp.constraint(self.init_action_constraint, u0, "==", a0)
-
-        # remove upper/lower bound on initial action in Q, since it is constrained as a0
         if remove_bounds_on_initial_action:
             for name, a in mpc.first_actions.items():
                 na_ = a.size1()
                 Q.nlp.remove_variable_bounds(name, "both", ((r, 0) for r in range(na_)))
 
+        # for V, add the cost perturbation parameter (only if gradient-based)
+        if self._exploration.mode == "gradient-based":
+            perturbation = V.nlp.parameter(self.cost_perturbation_parameter, (na, 1))
+            f = V.nlp.f
+            if mpc.is_wrapped(wrappers.NlpScaling):
+                f = mpc.scale(f)
+            V.nlp.minimize(f + cs.dot(perturbation, u0))
+
         # invalidate caches for V and Q since some modifications have been done
         for nlp in (V, Q):
             nlp_ = nlp
             while nlp_ is not nlp_.unwrapped:
                 invalidate_caches_of(nlp_)
                 nlp_ = nlp_.nlp
             invalidate_caches_of(nlp_.unwrapped)
```

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/agents/common/globopt_learning_agent.py` & `mpcrl-1.2.1rc1/src/mpcrl/agents/common/globopt_learning_agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,18 +26,25 @@
 
         Parameters
         ----------
         optimizer : GradientFreeOptimizer
             A gradient-free optimizer to ask for parameters and tell the values of the
             objective function.
         kwargs
-            Additional arguments to be passed to `LearningAgent` (with the exclusion of
-            the `update_strategy` argument, which is always set to update at the end of
-            each episode).
+            Additional arguments to be passed to `LearningAgent`.
+
+            Note: the following kwargs are not yet supported
+             - "experience": usually, GO strategies do not require experience replay
+             - "update_strategy": updates are fixed at the end of each episode
         """
+        for key in ("experience", "update_strategy"):
+            if key in kwargs:
+                raise ValueError(
+                    f"{self.__class__.__name__} does not yet support `{key}` kwargs."
+                )
         self.optimizer = optimizer
         super().__init__(update_strategy=UpdateStrategy(1, "on_episode_end"), **kwargs)
         self.optimizer.set_learnable_parameters(self._learnable_pars)
 
     def train(self, *args: Any, **kwargs: Any) -> Any:
         # prime the initial value of the learnable parameters by asking it to the
         # optimizer. This is the usual way to start Global Optimization strategies,
```

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/agents/common/learning_agent.py` & `mpcrl-1.2.1rc1/src/mpcrl/agents/common/learning_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from abc import ABC, abstractmethod
 from collections.abc import Collection, Iterable
 from typing import Any, Callable, Generic, Optional, TypeVar, Union
 
 import numpy as np
 import numpy.typing as npt
 from gymnasium import Env
+from gymnasium.spaces import Box
 
 from ...core.callbacks import LearningAgentCallbackMixin
-from ...core.exploration import ExplorationStrategy
+from ...core.experience import ExperienceReplay
 from ...core.parameters import LearnableParametersDict
 from ...core.update import UpdateStrategy
 from ...util.seeding import RngType, mk_seed
 from .agent import ActType, Agent, ObsType, SymType, _update_dicts
 
 ExpType = TypeVar("ExpType")
 
@@ -35,15 +36,15 @@
     Note: this class makes no assumptions on the learning methodology used to update the
     MPC's learnable parameters."""
 
     def __init__(
         self,
         update_strategy: Union[int, UpdateStrategy],
         learnable_parameters: LearnableParametersDict[SymType],
-        exploration: Optional[ExplorationStrategy] = None,
+        experience: Union[None, int, ExperienceReplay[ExpType]] = None,
         **kwargs: Any,
     ) -> None:
         """Instantiates the learning agent.
 
         Parameters
         ----------
         update_strategy : UpdateStrategy or int
@@ -51,42 +52,67 @@
             with. If an `int` is passed, then the default strategy that updates every
             `n` env's steps is used (where `n` is the argument passed); otherwise, an
             instance of `UpdateStrategy` can be passed to specify these in more details.
         learnable_parameters : LearnableParametersDict
             A special dict containing the learnable parameters of the MPC, together with
             their bounds and values. This dict is complementary with `fixed_parameters`,
             which contains the MPC parameters that are not learnt by the agent.
-        exploration : ExplorationStrategy, optional
-            Exploration strategy for inducing exploration in the MPC policy. By default
-            `None`, in which case `NoExploration` is used in the fixed-MPC agent.
+        experience : int or ExperienceReplay, optional
+            The container for experience replay memory. If `None` is passed, then a
+            memory with length 1 is created, i.e., it keeps only the latest memory
+            transition. If an integer `n` is passed, then a memory with the length `n`
+            is created and with sample size `n`.
         kwargs
             Additional arguments to be passed to `Agent`.
         """
         Agent.__init__(self, **kwargs)
         LearningAgentCallbackMixin.__init__(self)
         self._raises: bool = True
         self._learnable_pars = learnable_parameters
-        if exploration is not None:
-            self._exploration = exploration
+        if experience is None:
+            experience = ExperienceReplay(maxlen=1)
+        elif isinstance(experience, int):
+            experience = ExperienceReplay(maxlen=experience, sample_size=experience)
+        self._experience = experience
         if not isinstance(update_strategy, UpdateStrategy):
             update_strategy = UpdateStrategy(update_strategy, "on_timestep_end")
         self._update_strategy = update_strategy
         self._updates_enabled = True
         self.establish_callback_hooks()
 
     @property
+    def experience(self) -> ExperienceReplay[ExpType]:
+        """Gets the experience replay memory of the agent."""
+        return self._experience
+
+    @property
     def update_strategy(self) -> UpdateStrategy:
         """Gets the update strategy of the agent."""
         return self._update_strategy
 
     @property
     def learnable_parameters(self) -> LearnableParametersDict[SymType]:
         """Gets the parameters of the MPC that can be learnt by the agent."""
         return self._learnable_pars
 
+    def reset(self, seed: RngType = None) -> None:
+        """Resets agent's internal variables, exploration and experience's RNG"""
+        super().reset(seed)
+        self.experience.reset(seed)
+
+    def store_experience(self, item: ExpType) -> None:
+        """Stores the given item in the agent's memory for later experience replay.
+
+        Parameters
+        ----------
+        item : experience-type
+            Item to be stored in memory.
+        """
+        self._experience.append(item)
+
     def evaluate(self, *args: Any, **kwargs: Any) -> npt.NDArray[np.floating]:
         self._updates_enabled = False
         return super().evaluate(*args, **kwargs)
 
     def train(
         self,
         env: Env[ObsType, ActType],
@@ -121,14 +147,16 @@
         ------
         MpcSolverError or MpcSolverWarning
             Raises the error or the warning (depending on `raises`) if any of the MPC
             solvers fail.
         UpdateError or UpdateWarning
             Raises the error or the warning (depending on `raises`) if the update fails.
         """
+        if hasattr(env, "action_space"):
+            assert isinstance(env.action_space, Box), "Env action space must be a Box,"
         rng = np.random.default_rng(seed)
         self.reset(rng)
         self._updates_enabled = True
         self._raises = raises
         returns = np.zeros(episodes, float)
 
         self.on_training_start(env)
@@ -206,32 +234,27 @@
         ------
         MpcSolverError or MpcSolverWarning
             Raises the error or the warning (depending on `raises`) if any of the MPC
             solvers fail.
         UpdateError or UpdateWarning
             Raises the error or the warning (depending on `raises`) if the update fails.
         """
-        # TODO: implement the agent's `EvalWrapper` and use that to evaluate the
-        # agent's performance during off-policy training.
-
-        # TODO: `train` will need a rehaul, right? it will need to collect offpolicy
-
         rng = np.random.default_rng(seed)
         self.reset(rng)
         self._raises = raises
         env_proxy = "off-policy"
 
         self._updates_enabled = True
         self.on_training_start(env_proxy)
         for episode, rollout in enumerate(episode_rollouts):
             self.on_episode_start(env_proxy, episode, float("nan"))
             self.train_one_rollout(rollout, episode, raises)
             self.on_episode_end(env_proxy, episode, float("nan"))
 
-        self.on_training_end(env_proxy, [])
+        self.on_training_end(env_proxy, np.empty(0))
 
     def train_one_rollout(
         self, rollout: Iterable[Any], episode: int, raises: bool = True
     ) -> None:
         """Train the agent in an off-policy manner on the given rollout.
 
         Parameters
@@ -268,34 +291,27 @@
             In case the update fails, an error message is returned to be raised as error
             or warning; otherwise, `None` is returned.
         """
 
     def establish_callback_hooks(self) -> None:
         super().establish_callback_hooks()
         # hook exploration (only if necessary)
-        exploration_hook: Optional[str] = getattr(self._exploration, "hook", None)
+        exploration_hook = self._exploration.hook
         if exploration_hook is not None:
             self.hook_callback(
                 repr(self._exploration), exploration_hook, self._exploration.step
             )
         # hook updates (always necessary)
-        assert self._update_strategy.hook in {
-            "on_episode_end",
-            "on_timestep_end",
-        }, "Updates can be hooked only to `episode_end` or `on_timestep_end`."
+        update_hook = self._update_strategy.hook
         func: Callable[..., None] = (
             (lambda _, e, __: self._check_and_perform_update(e, None))
-            if self._update_strategy.hook == "on_episode_end"
+            if update_hook == "on_episode_end"
             else (lambda _, e, t: self._check_and_perform_update(e, t))
         )
-        self.hook_callback(
-            repr(self._update_strategy),
-            self._update_strategy.hook,
-            func,
-        )
+        self.hook_callback(repr(self._update_strategy), update_hook, func)
 
     def _check_and_perform_update(self, episode: int, timestep: Optional[int]) -> None:
         """Internal utility to check if an update is due and perform it."""
         if not self._updates_enabled or not self._update_strategy.can_update():
             return
         update_msg = self.update()
         if update_msg is not None:
```

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/agents/common/offpolicy_rl_agent copy.py` & `mpcrl-1.2.1rc1/src/mpcrl/agents/common/rl_learning_agent.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/agents/lstd_dpg.py` & `mpcrl-1.2.1rc1/src/mpcrl/agents/lstd_dpg.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 import numpy.typing as npt
 from csnlp.wrappers import Mpc, NlpSensitivity
 from gymnasium import Env
 from typing_extensions import TypeAlias
 
 from ..core.experience import ExperienceReplay
-from ..core.exploration import ExplorationStrategy
+from ..core.exploration import ExplorationStrategy, NoExploration
 from ..core.parameters import LearnableParametersDict
 from ..core.update import UpdateStrategy
 from ..core.warmstart import WarmStartStrategy
 from ..optim.gradient_based_optimizer import GradientBasedOptimizer
 from ..util.math import monomials_basis_function
 from .common.agent import ActType, ObsType, SymType
 from .common.rl_learning_agent import LrType, RlLearningAgent
@@ -54,23 +54,24 @@
     def __init__(
         self,
         mpc: Mpc[SymType],
         update_strategy: Union[int, UpdateStrategy],
         discount_factor: float,
         optimizer: GradientBasedOptimizer,
         learnable_parameters: LearnableParametersDict[SymType],
+        exploration: Optional[ExplorationStrategy],
         fixed_parameters: Union[
             None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]
         ] = None,
-        exploration: Optional[ExplorationStrategy] = None,
         experience: Union[None, int, ExperienceReplay[ExpType]] = None,
         warmstart: Union[
             Literal["last", "last-successful"], WarmStartStrategy
         ] = "last-successful",
-        rollout_length: Optional[int] = None,
+        hessian_type: Literal["none", "natural"] = "none",
+        rollout_length: int = -1,
         record_policy_performance: bool = False,
         record_policy_gradient: bool = False,
         state_features: Optional[cs.Function] = None,
         linsolver: Literal["csparse", "mldivide"] = "csparse",
         ridge_regression_regularization: float = 1e-6,
         use_last_action_on_fail: bool = False,
         name: Optional[str] = None,
@@ -99,22 +100,22 @@
             A gradient-based optimizer (e.g., `mpcrl.optim.GradientDescent`) to compute
             the updates of the learnable parameters, based on the current gradient-based
             RL algorithm.
         learnable_parameters : LearnableParametersDict
             A special dict containing the learnable parameters of the MPC, together with
             their bounds and values. This dict is complementary with `fixed_parameters`,
             which contains the MPC parameters that are not learnt by the agent.
+        exploration : ExplorationStrategy, optional
+            Exploration strategy for inducing exploration in the MPC policy (it is
+            mandatory to explore in DPG).
         fixed_parameters : dict[str, array_like] or collection of, optional
             A dict (or collection of dict, in case of `csnlp.MultistartNlp`) whose keys
             are the names of the MPC parameters and the values are their corresponding
             values. Use this to specify fixed parameters, that is, non-learnable. If
             `None`, then no fixed parameter is assumed.
-        exploration : ExplorationStrategy, optional
-            Exploration strategy for inducing exploration in the MPC policy. By default
-            `None`, in which case `NoExploration` is used in the fixed-MPC agent.
         experience : int or ExperienceReplay, optional
             The container for experience replay memory. If `None` is passed, then a
             memory with length 1 is created, i.e., it keeps only the latest memory
             transition. If an integer `n` is passed, then a memory with the length `n`
             is created and with sample size `n`.
             In case of LSTD DPG, each memory item is obtain from a single rollout, and
             is a 4-tuple that contains: costs, state vector features (Phi), Psi (a
@@ -133,22 +134,29 @@
             successful solution is used to warm start the solver for the next iteration.
             If `last`, the last solution is used, regardless of success or failure.
             Furthermoer, a `WarmStartStrategy` object can be passed to specify a
             strategy for generating multiple warmstart points for the NLP. This is
             useful to generate multiple initial conditions for very non-convex problems.
             Can only be used with an MPC that has an underlying multistart NLP problem
             (see `csnlp.MultistartNlp`).
+        hessian_type : {'none', 'natural'}, optional
+            The type of hessian to use in this (potentially) second-order algorithm.
+            If 'none', no second order information is used. If `natural`, the Fisher
+            information matrix is used to perform a natural policy gradient update. This
+            option must be in accordance with the choice of `optimizer`, that is, if the
+            optimizer does not use second order information, then this option must be
+            set to `none`.
         rollout_length : int, optional
-            Time-step length of a closed-loop simulation, which defines a complete
-            trajectory of the states, and is saved in the experience as a single item
-            (since LSTD DPG needs to draw samples of trajectories). In case the env is
-            episodic, it can be `None`, in which case the rollout length coincides with
-            the episode's. In case the env is not episodic, i.e., it never terminates, a
-            rollout length must be given in order to save the current trajectory as an
-            atomic item in memory.
+            Number of steps of each closed-loop simulation, which defines a complete
+            trajectory of the states (i.e., a rollout), and is saved in the experience
+            as a single item (since LSTD DPG needs to draw samples of trajectories). In
+            case the env is episodic, it can be `-1`, in which case the rollout length
+            coincides with the episode's length. In case the env is not episodic, i.e.,
+            it never terminates, a length `>0` must be given in order to know when to
+            save the current trajectory as an atomic item in memory.
         record_policy_performance: bool, optional
             If `True`, the performance of each rollout is stored in the field
             `policy_performances`, which otherwise is `None`. By default, does not
             record them.
         record_policy_gradient: bool, optional
             If `True`, the (estimated) policy gradient of each update is stored in the
             field `policy_gradients`, which otherwise is `None`. By default, does not
@@ -177,15 +185,23 @@
              * if `True`, the action from the last successful call to the MPC is
                returned instead (if the MPC has been solved at least once successfully).
 
             By default, `False`.
         name : str, optional
             Name of the agent. If `None`, one is automatically created from a counter of
             the class' instancies.
+
+        Raises
+        ------
+        ValueError
+            If the exploration strategy is `None` or an instance of `NoExploration`, as
+            DPG requires exploration.
         """
+        if exploration is None or isinstance(exploration, NoExploration):
+            raise ValueError("DPG requires exploration, but none was provided.")
         # change default update hook to 'on_episode_end'
         if not isinstance(update_strategy, UpdateStrategy):
             update_strategy = UpdateStrategy(update_strategy, "on_episode_end")
         super().__init__(
             mpc=mpc,
             update_strategy=update_strategy,
             discount_factor=discount_factor,
@@ -194,22 +210,23 @@
             fixed_parameters=fixed_parameters,
             exploration=exploration,
             experience=experience,
             warmstart=warmstart,
             use_last_action_on_fail=use_last_action_on_fail,
             name=name,
         )
+        self.hessian_type = hessian_type
         self._sensitivity = self._init_sensitivity(linsolver)
         self._Phi = (
             monomials_basis_function(mpc.ns, 0, 2)
             if state_features is None
             else state_features
         )
-        self.ridge_regression_regularization = ridge_regression_regularization
-        self.rollout_length = rollout_length or float("+inf")
+        self.regularization = ridge_regression_regularization
+        self.rollout_length = rollout_length
         self._rollout: list[
             tuple[
                 ObsType,
                 ActType,
                 SupportsFloat,
                 ObsType,
                 npt.NDArray[np.floating],
@@ -220,37 +237,56 @@
         )
         self.policy_gradients: Optional[list[npt.NDArray[np.floating]]] = (
             [] if record_policy_gradient else None
         )
 
     def update(self) -> Optional[str]:
         sample = self.experience.sample()
-        dJdtheta = _estimate_gradient_update(
-            sample, self.discount_factor, self.ridge_regression_regularization
-        )
+        if self.hessian_type == "natural":
+            dJdtheta, fisher_hessian = _estimate_gradient_update(
+                sample, self.discount_factor, self.regularization, True
+            )
+        else:
+            dJdtheta = _estimate_gradient_update(
+                sample, self.discount_factor, self.regularization, False
+            )
+            fisher_hessian = None
         if self.policy_gradients is not None:
             self.policy_gradients.append(dJdtheta)
-        return self.optimizer.update(dJdtheta)
+        return self.optimizer.update(dJdtheta, fisher_hessian)
 
     def train_one_episode(
         self,
         env: Env[ObsType, ActType],
         episode: int,
         init_state: ObsType,
         raises: bool = True,
     ) -> float:
         truncated = terminated = False
         timestep = 0
         rewards = 0.0
         state = init_state
+        rollout_length = self.rollout_length
+        action_space = getattr(env, "action_space", None)
+        gradient_based_exploration = self.exploration.mode == "gradient-based"
+        action_keys = self.V.actions.keys()
 
         while not (truncated or terminated):
-            # compute V(s) (perturbed and not perturbed)
-            action, sol = self.state_value(state, False)
-            action_opt, sol_opt = self.state_value(state, True)
+            # compute V(s)
+            action, sol = self.state_value(state, False, action_space=action_space)
+            if gradient_based_exploration:
+                # NOTE: if the exploration affects the gradient, unfortunately we have
+                # to solve again the NLP (but deterministically this time)
+                action_opt, sol_opt = self.state_value(
+                    state, True, action_space=action_space
+                )
+            else:
+                # otherwise, just retrieve manually the unperturbed optimal action
+                action_opt = cs.vertcat(*(sol.vals[u][:, 0] for u in action_keys))
+                sol_opt = sol
 
             # step the system with the action just computed
             state_new, cost, truncated, terminated, _ = env.step(action)
             self.on_env_step(env, episode, timestep)
 
             # store transition in experience
             if sol.success and sol_opt.success:
@@ -268,27 +304,29 @@
             # increase counters
             state = state_new
             rewards += float(cost)
             timestep += 1
 
             # first, check if current rollout has reached its length, and only then
             # invoke on_timestep_end (as it might trigger an update)
-            if len(self._rollout) >= self.rollout_length:
+            if rollout_length > 0 and len(self._rollout) >= rollout_length:
                 self._consolidate_rollout_into_memory()
             self.on_timestep_end(env, episode, timestep)
 
         # consolidate rollout at the end of episode, if no length was specified
-        if self.rollout_length == float("+inf"):
+        if rollout_length <= 0:
             self._consolidate_rollout_into_memory()
         return rewards
 
     def _init_sensitivity(self, linsolver: str) -> Callable[[cs.DM, int], np.ndarray]:
         """Internal utility to compute the derivatives w.r.t. the learnable parameters
         and other functions in order to estimate the policy gradient."""
-        assert self.optimizer._order == 1, "Expected 1st-order optimizer."
+        assert (self.hessian_type == "none" and self.optimizer._order == 1) or (
+            self.hessian_type == "natural" and self.optimizer._order == 2
+        ), "expected 1st-order (2nd-order) optimizer with `none` (`natural`) hessian"
         nlp = self._V.nlp
         y = nlp.primal_dual
         theta = cs.vvcat(self._learnable_pars.sym.values())
         u0 = cs.vcat(self._V.first_actions.values())
         x_lam_p = cs.vertcat(nlp.primal_dual, nlp.p)
 
         # compute first bunch of derivatives
@@ -336,16 +374,15 @@
         N, S, E, L, vals = _consolidate_rollout(self._rollout, self._V.ns, self._V.na)
         self._rollout.clear()
 
         # compute Phi, dpidtheta, Psi, and CAFA weight v
         Phi = np.ascontiguousarray(self._Phi(S.T).elements()).reshape(N + 1, -1)
         dpidtheta = self._sensitivity(vals, N)
         Psi = (dpidtheta @ E).reshape(N, dpidtheta.shape[1])
-        R = self.ridge_regression_regularization
-        v = _compute_cafa_weight_v(Phi, L, self.discount_factor, R)
+        v = _compute_cafa_weight_v(Phi, L, self.discount_factor, self.regularization)
 
         # save to experience
         self.store_experience((L, Phi, Psi, dpidtheta, v))
         if self.policy_performances is not None:
             self.policy_performances.append(L.sum())
 
 
@@ -402,22 +439,36 @@
     A = Psi.T @ Psi
     b = Psi.T @ (L + Phi_diff @ v)
     R = regularization * np.eye(A.shape[0])
     return np.linalg.solve(A.T @ A + R, A.T @ b)
 
 
 def _estimate_gradient_update(
-    sample: Iterator[ExpType], discount_factor: float, regularization: float
-) -> np.ndarray:
-    """Internal utility to estimate the gradient of the policy."""
+    sample: Iterator[ExpType],
+    discount_factor: float,
+    regularization: float,
+    return_fisher_hessian: bool,
+) -> Union[np.ndarray, tuple[np.ndarray, np.ndarray]]:
+    """Internal utility to estimate the gradient of the policy and possibly the
+    Fisher information matrix as well."""
     # compute average v and w
     sample_ = list(sample)  # load whole iterator into a list
     v = np.mean([o[4] for o in sample_], 0)
-    w_list = [
+    w_ = [
         _compute_cafa_weight_w(Phi, Psi, L, v, discount_factor, regularization)
         for L, Phi, Psi, _, _ in sample_
     ]
-    w = np.mean(w_list, 0)
+    w = np.mean(w_, 0)
 
-    # compute policy gradient estimate
-    dJdtheta_list = [(o[3] @ o[3].transpose((0, 2, 1))).sum(0) @ w for o in sample_]
-    return np.mean(dJdtheta_list, 0)
+    if return_fisher_hessian:
+        # compute both policy gradient and Fisher information matrix
+        fisher_hess_ = []
+        dJdtheta_ = []
+        for _, _, _, dpidtheta, _ in sample_:
+            F = (dpidtheta @ dpidtheta.transpose((0, 2, 1))).sum(0)
+            fisher_hess_.append(F)
+            dJdtheta_.append(F @ w)
+        return np.mean(dJdtheta_, 0), np.mean(fisher_hess_, 0)
+
+    # compute only policy gradient estimate
+    dJdtheta_ = [(o[3] @ o[3].transpose((0, 2, 1))).sum(0) @ w for o in sample_]
+    return np.mean(dJdtheta_, 0)
```

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/agents/lstd_q_learning.py` & `mpcrl-1.2.1rc1/src/mpcrl/agents/lstd_q_learning.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 from ..core.parameters import LearnableParametersDict
 from ..core.update import UpdateStrategy
 from ..core.warmstart import WarmStartStrategy
 from ..optim.gradient_based_optimizer import GradientBasedOptimizer
 from .common.agent import ActType, ObsType, SymType
 from .common.rl_learning_agent import LrType, RlLearningAgent
 
-ExpType: TypeAlias = tuple[
-    npt.NDArray[np.floating],  # gradient of Bellman residuals w.r.t. theta
-    npt.NDArray[np.floating],  # (approximate) hessian of Bellman residuals w.r.t. theta
+# the experience buffer contains the gradient and, possibly, the hessian of the Bellman
+# residuals w.r.t. the learnable parameters theta
+ExpType: TypeAlias = Union[
+    npt.NDArray[np.floating], tuple[npt.NDArray[np.floating], npt.NDArray[np.floating]]
 ]
 
 
 class LstdQLearningAgent(
     RlLearningAgent[SymType, ExpType, LrType], Generic[SymType, LrType]
 ):
     """Second-order Least-Squares Temporal Difference (LSTD) Q-learning agent, as first
@@ -114,15 +115,15 @@
             successful solution is used to warm start the solver for the next iteration.
             If `last`, the last solution is used, regardless of success or failure.
             Furthermoer, a `WarmStartStrategy` object can be passed to specify a
             strategy for generating multiple warmstart points for the NLP. This is
             useful to generate multiple initial conditions for very non-convex problems.
             Can only be used with an MPC that has an underlying multistart NLP problem
             (see `csnlp.MultistartNlp`).
-        hessian_type : 'none', 'approx' or 'full', optional
+        hessian_type : {'none', 'approx', 'full'}, optional
             The type of hessian to use in this (potentially) second-order algorithm.
             If 'none', no second order information is used. If `approx`, an easier
             approximation of it is used; otherwise, the full hessian is computed but
             this is much more expensive. This option must be in accordance with the
             choice of `optimizer`, that is, if the optimizer does not use second order
             information, then this option must be set to `none`.
         record_td_errors: bool, optional
@@ -162,50 +163,53 @@
         )
         self.hessian_type = hessian_type
         self._sensitivity = self._init_sensitivity(hessian_type)
         self.td_errors: Optional[list[float]] = [] if record_td_errors else None
 
     def update(self) -> Optional[str]:
         sample = self.experience.sample()
-        gradients = []
-        hessians = []
-        for g, H in sample:
-            gradients.append(g)
-            hessians.append(H)
+        if self.hessian_type == "none":
+            gradient = np.mean(list(sample), 0)
+            return self.optimizer.update(gradient)
+
+        gradients, hessians = zip(*sample)
         gradient = np.mean(gradients, 0)
-        hessian = np.mean(hessians, 0) if self.hessian_type != "none" else None
+        hessian = np.mean(hessians, 0)
         return self.optimizer.update(gradient, hessian)
 
     def train_one_episode(
         self,
         env: Env[ObsType, ActType],
         episode: int,
         init_state: ObsType,
         raises: bool = True,
     ) -> float:
         truncated = terminated = False
         timestep = 0
         rewards = 0.0
         state = init_state
+        action_space = getattr(env, "action_space", None)
 
         # solve for the first action
-        action, solV = self.state_value(state, False)
+        action, solV = self.state_value(state, False, action_space=action_space)
         if not solV.success:
             self.on_mpc_failure(episode, None, solV.status, raises)
 
         while not (truncated or terminated):
             # compute Q(s,a)
             solQ = self.action_value(state, action)
 
             # step the system with action computed at the previous iteration
             new_state, cost, truncated, terminated, _ = env.step(action)
             self.on_env_step(env, episode, timestep)
 
             # compute V(s+) and store transition
-            new_action, solV = self.state_value(new_state, False)
+            new_action, solV = self.state_value(
+                new_state, False, action_space=action_space
+            )
             if not self._try_store_experience(cost, solQ, solV):
                 self.on_mpc_failure(
                     episode, timestep, f"{solQ.status} (Q); {solV.status} (V)", raises
                 )
 
             # increase counters
             state = new_state
@@ -238,15 +242,14 @@
     def _init_sensitivity(
         self, hessian_type: Literal["none", "approx", "full"]
     ) -> Union[
         Callable[[cs.DM], np.ndarray], Callable[[cs.DM], tuple[np.ndarray, np.ndarray]]
     ]:
         """Internal utility to compute the derivative of Q(s,a) w.r.t. the learnable
         parameters, a.k.a., theta."""
-        assert hessian_type in ("none", "approx", "full"), "Invalid hessian type."
         order = self.optimizer._order
         theta = cs.vvcat(self._learnable_pars.sym.values())
         nlp = self._Q.nlp
         x_lam_p = cs.vertcat(nlp.primal_dual, nlp.p)
 
         # compute first order sensitivity
         snlp = NlpSensitivity(self._Q.nlp, theta)
@@ -293,25 +296,26 @@
 
     def _try_store_experience(
         self, cost: SupportsFloat, solQ: Solution[SymType], solV: Solution[SymType]
     ) -> bool:
         """Internal utility that tries to store the gradient and hessian for the current
         transition in memory, if both V and Q were successful; otherwise, does not store
         it. Returns whether it was successful or not."""
-        if solQ.success and solV.success:
+        success = solQ.success and solV.success
+        if success:
             sol_values = solQ.all_vals
             td_error = cost + self.discount_factor * solV.f - solQ.f
             if self.hessian_type == "none":
                 dQ = self._sensitivity(sol_values)
-                hessian = np.nan
+                gradient = -td_error * dQ
+                self.store_experience(gradient)
             else:
                 dQ, ddQ = self._sensitivity(sol_values)
+                gradient = -td_error * dQ
                 hessian = np.multiply.outer(dQ, dQ) - td_error * ddQ
-            gradient = -td_error * dQ
-            self.store_experience((gradient, hessian))
-            success = True
+                self.store_experience((gradient, hessian))
         else:
             td_error = np.nan
-            success = False
+
         if self.td_errors is not None:
             self.td_errors.append(td_error)
         return success
```

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/core/callbacks.py` & `mpcrl-1.2.1rc1/src/mpcrl/core/callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     Particularly touchy is when the state is set, and the hooks need to be reestablished
     automatically. In fact, if the old hooks are used, the new object (created from the
     state) would reference callbacks belonging to the old agent. In this way, the
     callbacks are linked to the new instance.
     """
 
     def __init__(self) -> None:
-        self._hooks: dict[str, list[tuple[str, Callable[..., None]]]] = {}
+        self._hooks: dict[str, dict[str, Callable[..., None]]] = {}
 
     def __setstate__(
         self,
         state: Union[
             None, dict[str, Any], tuple[Optional[dict[str, Any]], dict[str, Any]]
         ],
     ) -> None:
```

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/core/errors.py` & `mpcrl-1.2.1rc1/src/mpcrl/core/errors.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/core/experience.py` & `mpcrl-1.2.1rc1/src/mpcrl/core/experience.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,22 +28,35 @@
         ----------
         iterable : Iterable of T, optional
             Initial items to be inserted in the container. By default, empty.
         maxlen : int, optional
             Maximum length/capacity of the memory. If `None`, the deque has no maximum
             size, which is the default behaviour.
         sample_size : int or float, optional
-            Size (or percentage of replay `maxlen`) of the experience replay items to
-            draw when performing an update. By default, one item per sampling is drawn.
+            Size (as integer, or float percentage of `maxlen`) of the experience replay
+            items to draw when performing an update. By default, one item per sampling
+            is drawn. If a float percentage, `maxlen` must be provided.
         include_latest : int or float, optional
-            Size (or percentage of `sample_size`) dedicated to including the latest
-            experience transitions. By default, 0, i.e., no last item is included.
+            Size (as integer, or float percentage of `sample_size`) dedicated to
+            including the latest experience items. By default, 0, i.e., no last item is
+            included.
         seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
             Seed for the random number generator. By default, `None`.
+
+        Raises
+        ------
+        TypeError
+            Raises if `sample_size` is a float (a percentage of the maximum length), but
+            `maxlen` is `None`, since it is impossible to compute the percentage of an
+            unknown quantity.
         """
+        if isinstance(sample_size, float) and maxlen is None:
+            raise TypeError(
+                "Cannot compute the percentage of an unknown quantity (maxlen is None)."
+            )
         super().__init__(iterable, maxlen=maxlen)
         self.sample_size = sample_size
         self.include_latest = include_latest
         self.reset(seed)
 
     def reset(self, seed: RngType = None) -> None:
         """Resets the sampling RNG."""
@@ -52,29 +65,19 @@
     def sample(self) -> Iterator[ExpType]:
         """Samples the experience memory and yields the sampled items.
 
         Returns
         -------
         sample : iterator of T
             An iterable sample is yielded.
-
-        Raises
-        ------
-        TypeError
-            Raises if `sample_size` is a float (a percentage of the maximum length), but
-            `maxlen` is `None`, since it is impossible to compute the percentage of an
-            unknown quantity.
         """
         L = len(self)
         n = self.sample_size
         last_n = self.include_latest
         if isinstance(n, float):
-            assert (
-                self.maxlen is not None
-            ), "Maxlen is `None`; cannot use sample percentages."
             n = int(self.maxlen * n)
         n = min(max(n, 0), L)
         if isinstance(last_n, float):
             last_n = int(n * last_n)
         last_n = min(max(last_n, 0), n)
 
         # get last n indices and the sampled indices from the remaining
```

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/core/exploration.py` & `mpcrl-1.2.1rc1/src/mpcrl/core/exploration.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,58 @@
 import numpy.typing as npt
 
 from ..util.seeding import RngType
 from .schedulers import NoScheduling, Scheduler
 
 
 class ExplorationStrategy(ABC):
-    """Base class for exploration strategies such as greedy, epsilon-greeyd, etc."""
+    """Base class for exploration strategies such as greedy, epsilon-greedy, etc."""
+
+    def __init__(
+        self,
+        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
+        mode: Literal["gradient-based", "additive"] = "gradient-based",
+    ) -> None:
+        """Instantiates a generic exploration strategy.
+
+        Parameters
+        ----------
+        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
+            Specifies to which callback to hook, i.e., when to step the exploration's
+            schedulers (if any) to, e.g., decay the chances of exploring or the
+            perturbation strength (see `step` method also). The options are:
+             - `on_update` steps the exploration after each agent's update
+             - `on_episode_end` steps the exploration after each episode's end
+             - `on_timestep_end` steps the exploration after each env's timestep.
+
+            By default, 'on_update' is selected.
+        mode : {'gradient-based', 'additive'} optional
+            Mode of application of explorative perturbations to the MPC. If `additive`,
+            then the drawn pertubation is added to the optimal action computed by the
+            MPC. By default, `gradient-based` is selected, and in this mode the
+            pertubations enter  directly in the MPC objective and multiplied by the
+            first action, thus affecting its gradient.
+        """
+        super().__init__()
+        self._hook = hook
+        self._mode = mode
+
+    @property
+    def hook(
+        self,
+    ) -> Optional[Literal["on_update", "on_episode_end", "on_timestep_end"]]:
+        """Specifies to which callback to hook, i.e., when to step the exploration's
+        schedulers (if any) to, e.g., decay the chances of exploring or the perturbation
+        strength (see `step` method also). Can be `None` in case no hook is needed."""
+        return self._hook  # override this property if schedulers are used in the class
+
+    @property
+    def mode(self) -> Literal["gradient-based", "additive"]:
+        """Mode of application of explorative perturbations to the MPC."""
+        return self._mode
 
     @abstractmethod
     def can_explore(self) -> bool:
         """Computes whether, according to the exploration strategy, the agent should
         explore or not at the current instant.
 
         Returns
@@ -28,49 +71,68 @@
         """Updates the exploration strength and/or probability, in case the strategy
         supports them (usually, by decaying them over time)."""
 
     @abstractmethod
     def perturbation(self, *args: Any, **kwargs: Any) -> npt.NDArray[np.floating]:
         """Returns a random perturbation."""
 
+    def reset(self, _: RngType = None) -> None:
+        """Resets the exploration status, in case it is non-deterministic."""
+
     def __str__(self) -> str:
         return self.__class__.__name__
 
     def __repr__(self) -> str:
-        hook: Optional[str] = getattr(self, "hook", None)
-        if hook is None:
-            return self.__class__.__name__
-        return f"{self.__class__.__name__}(hook='{hook}')"
+        return f"{self.__class__.__name__}(hook={self.hook},mode={self.mode})"
 
 
 class NoExploration(ExplorationStrategy):
     """Strategy where no exploration is allowed at any time or, in other words, the
     policy is always deterministic (only based on the current state, and not perturbed).
     """
 
+    def __init__(self) -> None:
+        """Instiates a no-exploration strategy."""
+        super().__init__()
+        del self._hook, self._mode
+
+    @property
+    def hook(self) -> None:
+        """Returns `None`, since no exploration is allowed."""
+        return None
+
+    @property
+    def mode(self) -> None:
+        """Returns no mode."""
+        return None
+
     def can_explore(self) -> bool:
         return False
 
     def step(self, *_, **__) -> None:
         return
 
     def perturbation(self, *args: Any, **kwargs: Any) -> npt.NDArray[np.floating]:
         raise NotImplementedError(
             f"Perturbation not implemented in {self.__class__.__name__}"
         )
 
+    def __repr__(self) -> str:
+        return self.__class__.__name__ + "()"
+
 
 class GreedyExploration(ExplorationStrategy):
     """Fully greedy strategy for perturbing the policy, thus inducing exploration. This
     strategy always perturbs randomly the policy."""
 
     def __init__(
         self,
         strength: Union[Scheduler[npt.NDArray[np.floating]], npt.NDArray[np.floating]],
         hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
+        mode: Literal["gradient-based", "additive"] = "gradient-based",
         seed: RngType = None,
     ) -> None:
         """Initializes the greedy exploration strategy.
 
         Parameters
         ----------
         strength : scheduler or array/supports-algebraic-operations
@@ -84,38 +146,37 @@
             schedulers (if any) to, e.g., decay the chances of exploring or the
             perturbation strength (see `step` method also). The options are:
              - `on_update` steps the exploration after each agent's update
              - `on_episode_end` steps the exploration after each episode's end
              - `on_timestep_end` steps the exploration after each env's timestep.
 
             By default, 'on_update' is selected.
+        mode : {'gradient-based', 'additive'} optional
+            Mode of application of explorative perturbations to the MPC. If `additive`,
+            then the drawn pertubation is added to the optimal action computed by the
+            MPC. By default, `gradient-based` is selected, and in this mode the
+            pertubations enter  directly in the MPC objective and multiplied by the
+            first action, thus affecting its gradient.
         seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
             Number to seed the RNG engine used for randomizing the exploration. By
             default, `None`.
         """
-        super().__init__()
-        self._hook = hook
+        super().__init__(hook, mode)
         if not isinstance(strength, Scheduler):
             strength = NoScheduling[npt.NDArray[np.floating]](strength)
         self.strength_scheduler = strength
         self.reset(seed)
 
     @property
-    def hook(self) -> Optional[str]:
-        """Specifies to which callback to hook, i.e., when to step the exploration's
-        schedulers (if any) to, e.g., decay the chances of exploring or the perturbation
-        strength (see `step` method also). Can be `None` in case no hook is needed."""
+    def hook(
+        self,
+    ) -> Optional[Literal["on_update", "on_episode_end", "on_timestep_end"]]:
         # return hook only if the strength scheduler requires to be stepped
         return None if isinstance(self.strength_scheduler, NoScheduling) else self._hook
 
-    @property
-    def strength(self) -> npt.NDArray[np.floating]:
-        """Gets the current strength of the exploration strategy."""
-        return self.strength_scheduler.value
-
     def reset(self, seed: RngType = None) -> None:
         """Resets the exploration RNG."""
         self.np_random = np.random.default_rng(seed)
 
     def can_explore(self) -> bool:
         return True
 
@@ -143,31 +204,28 @@
         """
         return (
             getattr(self.np_random, method)(*args, **kwargs)
             * self.strength_scheduler.value
         )
 
     def __repr__(self) -> str:
-        hook = self.hook
-        hookstr = "None" if hook is None else f"'{hook}'"
-        return (
-            f"{self.__class__.__name__}(stn={self.strength_scheduler.value},"
-            f"hook={hookstr})"
-        )
+        stn = self.strength_scheduler.value
+        return f"{self.__class__.__name__}(stn={stn},hook={self.hook},mode={self.mode})"
 
 
 class EpsilonGreedyExploration(GreedyExploration):
     """Epsilon-greedy strategy for perturbing the policy, thus inducing exploration.
     This strategy only occasionally perturbs randomly the policy."""
 
     def __init__(
         self,
         epsilon: Union[Scheduler[float], float],
         strength: Union[Scheduler[npt.NDArray[np.floating]], npt.NDArray[np.floating]],
         hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
+        mode: Literal["gradient-based", "additive"] = "gradient-based",
         seed: RngType = None,
     ) -> None:
         """Initializes the epsilon-greedy exploration strategy.
 
         Parameters
         ----------
         epsilon : scheduler or float
@@ -183,54 +241,55 @@
             schedulers (if any) to, e.g., decay the chances of exploring or the
             perturbation strength (see `step` method also). The options are:
              - `on_update` steps the exploration after each agent's update
              - `on_episode_end` steps the exploration after each episode's end
              - `on_timestep_end` steps the exploration after each env's timestep.
 
             By default, 'on_update' is selected.
+        mode : {'gradient-based', 'additive'} optional
+            Mode of application of explorative perturbations to the MPC. If `additive`,
+            then the drawn pertubation is added to the optimal action computed by the
+            MPC. By default, `gradient-based` is selected, and in this mode the
+            pertubations enter  directly in the MPC objective and multiplied by the
+            first action, thus affecting its gradient.
         seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
             Number to seed the RNG engine used for randomizing the exploration. By
             default, `None`.
         """
-        super().__init__(strength, hook, seed)
+        super().__init__(strength, hook, mode, seed)
         if not isinstance(epsilon, Scheduler):
             epsilon = NoScheduling[float](epsilon)
         self.epsilon_scheduler = epsilon
 
     @property
-    def hook(self) -> Optional[str]:
+    def hook(
+        self,
+    ) -> Optional[Literal["on_update", "on_episode_end", "on_timestep_end"]]:
         # return hook only if the strength or epislon scheduler requires to be stepped
         return (
             None
             if isinstance(self.strength_scheduler, NoScheduling)
             and isinstance(self.epsilon_scheduler, NoScheduling)
             else self._hook
         )
 
-    @property
-    def epsilon(self) -> float:
-        """Gets the current probability of the exploration strategy."""
-        return self.epsilon_scheduler.value
-
     def can_explore(self) -> bool:
         return self.np_random.random() <= self.epsilon_scheduler.value
 
     def step(self, *_, **__) -> None:
         """Updates the exploration probability and strength according to their
         schedulers."""
         self.strength_scheduler.step()
         self.epsilon_scheduler.step()
 
     def __repr__(self) -> str:
-        hook = self.hook
-        hookstr = "None" if hook is None else f"'{hook}'"
-        return (
-            f"{self.__class__.__name__}(eps={self.epsilon_scheduler.value},"
-            f"stn={self.strength_scheduler.value},hook={hookstr})"
-        )
+        clsn = self.__class__.__name__
+        eps = self.epsilon_scheduler.value
+        stn = self.strength_scheduler.value
+        return f"{clsn}(eps={eps},stn={stn},hook={self.hook},mode={self.mode})"
 
 
 class StepWiseExploration(ExplorationStrategy):
     """Wrapper exploration class that enables a base exploration strategy to change only
     every N steps, thus yielding a step-wise strategy with steps of the given length.
     This is useful when, e.g., the exploration strategy must be kept constant across
     time for a number of steps.
@@ -259,24 +318,32 @@
         step_size : int
             Size of each step.
         stepwise_decay : bool, optional
             Enables the decay `step` to also be step-wise, i.e., applied only every N
             steps.
         """
         super().__init__()
+        del self._hook, self._mode
         self.base_exploration = base_exploration
         self.step_size = step_size
         self._explore_counter = 0
         self._step_counter = 0
         self._stepwise_decay = stepwise_decay
 
     @property
-    def hook(self) -> Optional[str]:
+    def hook(
+        self,
+    ) -> Optional[Literal["on_update", "on_episode_end", "on_timestep_end"]]:
         """Returns the hook of the base exploration strategy, if any."""
-        return getattr(self.base_exploration, "hook", None)
+        return self.base_exploration.hook
+
+    @property
+    def mode(self) -> Literal["gradient-based", "additive"]:
+        """Returns the mode of the base exploration strategy."""
+        return self.base_exploration.mode
 
     def can_explore(self) -> bool:
         # since this method is called at every timestep (when deterministic=False), we
         # decide here if the base exploration is frozen or not, i.e., if we are at the
         # new step or not
         self._explore_counter %= self.step_size
         if self._explore_counter == 0:
@@ -301,8 +368,10 @@
             return self._cached_perturbation
         self._cached_perturbation = self.base_exploration.perturbation(*args, **kwargs)
         return self._cached_perturbation
 
     def __repr__(self) -> str:
         clsn = self.__class__.__name__
         bclsn = self.base_exploration.__class__.__name__
-        return f"{clsn}(base={bclsn},step_size={self.step_size})"
+        h = self.hook
+        m = self.mode
+        return f"{clsn}(base={bclsn},step_size={self.step_size},hook={h},mode={m})"
```

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/core/parameters.py` & `mpcrl-1.2.1rc1/src/mpcrl/core/parameters.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/core/schedulers.py` & `mpcrl-1.2.1rc1/src/mpcrl/core/schedulers.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/core/update.py` & `mpcrl-1.2.1rc1/src/mpcrl/core/update.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/core/warmstart.py` & `mpcrl-1.2.1rc1/src/mpcrl/core/warmstart.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,88 +28,78 @@
         ----------
         warmstart: "last" or "last-successful", optional
             The warmstart strategy for the MPC's NLP. If `last-successful`, the last
             successful solution is used to warm start the solver for the next iteration.
             If `last`, the last solution is used, regardless of success or failure.
         structured_points : StructuredStartPoint, optional
             Class containing info on how to generate structured starting points for the
-            NLP. Note that its `multistarts` attribute will be overwritten with the
-            correct value of requested structured initial conditions.
-            If `None`, no structured point is generated.
+            NLP. If `None`, no structured point is generated.
         random_points : RandomStartPoints, optional
             Class containing info on how to generate random starting points for the NLP.
-            Note that its `multistarts` attribute will be overwritten with the
-            correct value of requested random initial conditions, and its `biases` will
-            be updated with the last successful solution.
-            If `None`, no random point is generated.
+            Its `biases` field will be automatically updated with the last successful
+            solution, unless disabled with `update_biases_for_random_points=False`). If
+            `None`, no random point is generated.
         update_biases_for_random_points : bool, optional
             If `True`, the random points are biased around the bias-values updated with
             the latest successful MPC solution. If `False`, the biases in
             `random_points` are not updated.
         seed : None, int, array of ints, SeedSequence, BitGenerator, Generator
             Seed for the random number generator. By default, `None`.
         """
         self.store_always = warmstart == "last"
         self.structured_points = structured_points
         self.random_points = random_points
         self.update_biases_for_random_points = update_biases_for_random_points
         self.reset(seed)
 
     @property
-    def can_generate(self) -> bool:
-        """Returns whether the warm start strategy can generate initial conditions."""
-        return self.structured_points is not None or self.random_points is not None
+    def n_points(self) -> int:
+        """Returns the number of both random and structured starting points."""
+        return (0 if self.random_points is None else self.random_points.multistarts) + (
+            0 if self.structured_points is None else self.structured_points.multistarts
+        )
 
     def reset(self, seed: RngType = None) -> None:
         """Resets the sampling RNG."""
-        self.np_random = np.random.default_rng(seed)
+        if self.random_points is not None:
+            self.random_points.np_random = np.random.default_rng(seed)
 
     def generate(
-        self,
-        n_struct: int,
-        n_rand: int,
-        biases: Optional[dict[str, npt.ArrayLike]] = None,
+        self, biases: Optional[dict[str, npt.ArrayLike]] = None
     ) -> Generator[dict[str, npt.ArrayLike], None, None]:
         """Generates initial conditions for the MPC's NLP.
 
         Parameters
         ----------
-        n_struct : int
-            The number of structured initial conditions to generate.
-        n_rand : int
-            The number of random initial conditions to generate.
         biases : dict of (str, array_like), optional
             Optional biases that can be used to update the random points' original
             biases. If `None` or `update_biases_for_random_points=False`, the original
             biases are kept constant. These do not affect the generation of structure
             points in any way.
 
         Yields
         ------
         Generator of dict of (str, array_like)
             Yields the initial conditions for the MPC's NLP.
         """
         to_be_chained = []
 
         if self.structured_points is not None:
-            self.structured_points.multistarts = n_struct
             to_be_chained.append(self.structured_points)
 
         if self.random_points is not None:
-            self.random_points.multistarts = n_rand
-            self.random_points.np_random = self.np_random
             if self.update_biases_for_random_points and biases is not None:
                 self.random_points.biases.update(biases)
             to_be_chained.append(self.random_points)
 
         return chain.from_iterable(to_be_chained)
 
     def __repr__(self) -> str:
-        nr = len(self.random_points) if self.random_points is not None else 0
-        ns = len(self.structured_points) if self.structured_points is not None else 0
+        nr = 0 if self.random_points is None else self.random_points.multistarts
+        ns = 0 if self.structured_points is None else self.structured_points.multistarts
         return (
             f"{self.__class__.__name__}(store_always={self.store_always},"
             f"random_points={nr},structured_points={ns})"
         )
 
     def __str__(self) -> str:
         return self.__repr__()
```

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/optim/adam.py` & `mpcrl-1.2.1rc1/src/mpcrl/optim/adam.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/optim/base_optimizer.py` & `mpcrl-1.2.1rc1/src/mpcrl/optim/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/optim/gradient_based_optimizer.py` & `mpcrl-1.2.1rc1/src/mpcrl/optim/gradient_based_optimizer.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/optim/gradient_descent.py` & `mpcrl-1.2.1rc1/src/mpcrl/optim/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/optim/gradient_free_optimizer.py` & `mpcrl-1.2.1rc1/src/mpcrl/optim/gradient_free_optimizer.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/optim/newton_method.py` & `mpcrl-1.2.1rc1/src/mpcrl/optim/newton_method.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/optim/rmsprop.py` & `mpcrl-1.2.1rc1/src/mpcrl/optim/rmsprop.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/util/control.py` & `mpcrl-1.2.1rc1/src/mpcrl/util/control.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/util/iters.py` & `mpcrl-1.2.1rc1/src/mpcrl/util/iters.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/util/math.py` & `mpcrl-1.2.1rc1/src/mpcrl/util/math.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/util/named.py` & `mpcrl-1.2.1rc1/src/mpcrl/util/named.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/util/seeding.py` & `mpcrl-1.2.1rc1/src/mpcrl/util/seeding.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/log.py` & `mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/log.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/record_updates.py` & `mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/record_updates.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/wrappers/agents/wrapper.py` & `mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Parameters
         ----------
         agent : Agent or subclass
             The agent to wrap.
         """
         SupportsDeepcopyAndPickle.__init__(self)
         CallbackMixin.__init__(self)
-        del self._hooks  # only keep one dict of hooks, i.e., the agent's one
+        del self._hooks  # keep only one dict of hooks, i.e., the agent's one
         self.agent = agent
         self._hooked_callbacks: dict[str, list[str]] = {}
         self.establish_callback_hooks()
 
     @property
     def unwrapped(self) -> Union[Agent[SymType], LearningAgent[SymType, ExpType]]:
         """'Returns the original agent of the wrapper."""
@@ -54,19 +54,24 @@
     ) -> None:
         """See `LearningAgent.hook_callback`."""
         # store the callback id for later removal via `detach_wrapper(s)`
         self._hooked_callbacks.setdefault(callbackname, []).append(attachername)
         self.unwrapped.hook_callback(attachername, callbackname, func)
 
     def detach_wrapper(
-        self,
+        self, recursive: bool = False
     ) -> Union[Agent[SymType], LearningAgent[SymType, ExpType], "Wrapper[SymType]"]:
-        """Detaches the wrapper from the agent, returning the wrapped agent. De facto,
+        """Detaches the wrapper from the agent, returning the unwrapped agent. De facto,
         this method detaches all the hooks attached by this wrapper.
 
+        Parameters
+        ----------
+        recursive : bool, optional
+            If `True`, detaches all the wrappers around the agent recursively.
+
         Returns
         -------
         Agent or Wrapper
             Returns the wrapped agent (or other wrapper) instance. This instance has no
             more active hooks attached by this wrapper.
         """
         hooks = self.unwrapped._hooks
@@ -80,29 +85,21 @@
 
             # if the callback has no more hooks, remove it
             if not hook_group:
                 hooks.pop(callbackname)
 
         # clear hooked callbacks tracking
         hooked_callbacks.clear()
-        return self.agent
-
-    def detach_wrappers(self) -> Union[Agent[SymType], LearningAgent[SymType, ExpType]]:
-        """Similar to `detach_wrapper`, but detaches all wrappers around the agent.
-
-        Returns
-        -------
-        Agent
-            Returns the wrapped agent instance. This instance has no more active hooks
-            attached by all the wrappers around it.
-        """
-        agent_ = self
-        while hasattr(agent_, "detach_wrapper") and callable(agent_.detach_wrapper):
-            agent_ = agent_.detach_wrapper()
-        return agent_
+        return (
+            self.agent.detach_wrapper(True)
+            if recursive
+            and hasattr(self.agent, "detach_wrapper")
+            and callable(self.agent.detach_wrapper)
+            else self.agent
+        )
 
     def __getattr__(self, name: str) -> Any:
         """Reroutes attributes to the wrapped agent instance."""
         if name.startswith("_"):
             raise AttributeError(f"Accessing private attribute '{name}' is prohibited.")
         return getattr(self.agent, name)
```

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/wrappers/envs/monitor_episodes.py` & `mpcrl-1.2.1rc1/src/mpcrl/wrappers/envs/monitor_episodes.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl/wrappers/envs/monitor_infos.py` & `mpcrl-1.2.1rc1/src/mpcrl/wrappers/envs/monitor_infos.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/src/mpcrl.egg-info/PKG-INFO` & `mpcrl-1.2.1rc1/src/mpcrl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcrl
-Version: 1.2.0rc4
+Version: 1.2.1rc1
 Summary: Reinforcement Learning with Model Predictive Control
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/mpc-reinforcement-learning
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues
 Keywords: reinforcement-learning,model-predictive-control,optimization,casadi
 Classifier: Programming Language :: Python
@@ -18,15 +18,15 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions>=4.5.0
 Requires-Dist: numba>=0.57.1
-Requires-Dist: csnlp>=1.5.10rc3
+Requires-Dist: csnlp>=1.5.10
 Requires-Dist: scipy>=1.11.0
 Requires-Dist: gymnasium>=0.28.1
 
 # Reinforcement Learning with Model Predictive Control
 
 **mpcrl** is a library for training model-based Reinforcement Learning (RL) agents with Model Predictive Control (MPC) as function approximation. This framework, also known as MPC-based RL, was first proposed in [[1]](#1) and has so far been shown effective in various applications and with different learning algorithms, e.g., [[2](#2),[3](#3)].
```

### Comparing `mpcrl-1.2.0rc4/src/mpcrl.egg-info/SOURCES.txt` & `mpcrl-1.2.1rc1/src/mpcrl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 src/mpcrl.egg-info/requires.txt
 src/mpcrl.egg-info/top_level.txt
 src/mpcrl/agents/lstd_dpg.py
 src/mpcrl/agents/lstd_q_learning.py
 src/mpcrl/agents/common/agent.py
 src/mpcrl/agents/common/globopt_learning_agent.py
 src/mpcrl/agents/common/learning_agent.py
-src/mpcrl/agents/common/offpolicy_rl_agent copy.py
 src/mpcrl/agents/common/rl_learning_agent.py
 src/mpcrl/core/__init__.py
 src/mpcrl/core/callbacks.py
 src/mpcrl/core/errors.py
 src/mpcrl/core/experience.py
 src/mpcrl/core/exploration.py
 src/mpcrl/core/parameters.py
@@ -33,14 +32,15 @@
 src/mpcrl/optim/rmsprop.py
 src/mpcrl/util/control.py
 src/mpcrl/util/iters.py
 src/mpcrl/util/math.py
 src/mpcrl/util/named.py
 src/mpcrl/util/seeding.py
 src/mpcrl/wrappers/agents/__init__.py
+src/mpcrl/wrappers/agents/evaluate.py
 src/mpcrl/wrappers/agents/log.py
 src/mpcrl/wrappers/agents/record_updates.py
 src/mpcrl/wrappers/agents/wrapper.py
 src/mpcrl/wrappers/envs/__init__.py
 src/mpcrl/wrappers/envs/monitor_episodes.py
 src/mpcrl/wrappers/envs/monitor_infos.py
 tests/test_agent.py
```

### Comparing `mpcrl-1.2.0rc4/tests/test_agent.py` & `mpcrl-1.2.1rc1/tests/test_agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,21 +105,32 @@
 
     def test_init__instantiates_V_and_Q_as_two_different_mpcs(self):
         agent = Agent(mpc=get_mpc(3, self.multistart_nlp))
         self.assertIsInstance(agent.Q, Mpc)
         self.assertIsInstance(agent.V, Mpc)
         self.assertIsNot(agent.Q, agent.V)
 
-    def test_init__instantiates_V_and_Q_correctly(self):
-        agent = Agent(mpc=get_mpc(3, self.multistart_nlp))
-        self.assertIn(agent.cost_perturbation_parameter, agent.V.parameters.keys())
-        self.assertNotIn(agent.cost_perturbation_parameter, agent.Q.parameters.keys())
-        self.assertIn(agent.init_action_parameter, agent.Q.parameters.keys())
+    @parameterized.expand([(None,), ("gradient-based",), ("additive",)])
+    def test_init__instantiates_V_and_Q_correctly(self, exploration_mode: str):
+        if exploration_mode is None:
+            exploration = E.NoExploration()
+        else:
+            exploration = E.GreedyExploration(0.5, mode=exploration_mode)
+        agent = Agent(mpc=get_mpc(3, self.multistart_nlp), exploration=exploration)
+
+        V_pars_keys = agent.V.parameters.keys()
+        Q_pars_keys = agent.Q.parameters.keys()
+        if exploration_mode is None or exploration_mode == "additive":
+            self.assertNotIn(agent.cost_perturbation_parameter, V_pars_keys)
+        else:
+            self.assertIn(agent.cost_perturbation_parameter, V_pars_keys)
+        self.assertNotIn(agent.cost_perturbation_parameter, Q_pars_keys)
+        self.assertIn(agent.init_action_parameter, Q_pars_keys)
         self.assertIn(agent.init_action_constraint, agent.Q.constraints.keys())
-        self.assertNotIn(agent.init_action_parameter, agent.V.parameters.keys())
+        self.assertNotIn(agent.init_action_parameter, V_pars_keys)
         self.assertNotIn(agent.init_action_constraint, agent.V.constraints.keys())
 
     def test_init__removes_bounds_on_initial_action_in_Q_correctly(self):
         mpc = get_mpc(3, self.multistart_nlp)
         mpc.unwrapped.remove_variable_bounds = Mock()
         agent = Agent(mpc=mpc, remove_bounds_on_initial_action=True)
         self.assertFalse(agent.V.remove_variable_bounds.called)
@@ -183,15 +194,16 @@
         }
         fixed_pars_ = (
             (fixed_pars.copy() for _ in range(starts))
             if multiple_pars
             else fixed_pars.copy()
         )
         mpc = get_mpc(horizon, self.multistart_nlp)
-        agent = Agent(mpc=mpc, fixed_parameters=fixed_pars_)
+        exploration = E.GreedyExploration(0.5, mode="gradient-based")
+        agent = Agent(mpc=mpc, fixed_parameters=fixed_pars_, exploration=exploration)
         mpc: Mpc[cs.SX] = getattr(agent, mpctype)
 
         s = {"y": 0, "v": 10, "m": 5e5}
         a = {"u1": 1, "u2": 2}
         if vector:
             s = cs.DM(s.values())
             a = cs.DM(a.values())
```

### Comparing `mpcrl-1.2.0rc4/tests/test_core.py` & `mpcrl-1.2.1rc1/tests/test_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 from itertools import product
 from random import shuffle
 from typing import Union
 from unittest.mock import Mock
 
 import casadi as cs
 import numpy as np
+from csnlp.multistart import RandomStartPoints, StructuredStartPoints
 from parameterized import parameterized
 
 from mpcrl import (
     ExperienceReplay,
     LearnableParameter,
     LearnableParametersDict,
     MpcSolverError,
     MpcSolverWarning,
     UpdateError,
     UpdateStrategy,
     UpdateWarning,
+    WarmStartStrategy,
 )
 from mpcrl import exploration as E
 from mpcrl import schedulers as S
 from mpcrl.core.errors import (
     raise_or_warn_on_mpc_failure,
     raise_or_warn_on_update_failure,
 )
@@ -81,17 +83,16 @@
         self.assertEqual(mem.maxlen, maxlen)
         self.assertNotIn(items[0], mem)
         self.assertIn(items[1], mem)
         self.assertIn(items[2], mem)
         self.assertIsInstance(mem.np_random, np.random.Generator)
 
     def test_sample__raises__with_no_maxlen_and_percentage_size(self):
-        mem = ExperienceReplay[tuple[np.ndarray, float]](maxlen=None, sample_size=0.0)
-        with self.assertRaises(AssertionError):
-            list(mem.sample())
+        with self.assertRaises(TypeError):
+            ExperienceReplay[tuple[np.ndarray, float]](maxlen=None, sample_size=0.0)
 
     @parameterized.expand([(0,), (float(0),)])
     def test_sample__with_zero_samples__returns_no_samples(self, n: Union[int, float]):
         mem = ExperienceReplay[tuple[np.ndarray, float]](maxlen=100, sample_size=n)
         self.assertListEqual(list(mem.sample()), [])
 
     @parameterized.expand([(10,), (0.1,)])
@@ -247,14 +248,21 @@
         )
         self.assertEqual(len(values_actual), steps_expected)
         self.assertEqual(len(values_expected), len(values_actual))
         np.testing.assert_array_equal(values_expected, values_actual)
 
 
 class TestExploration(unittest.TestCase):
+    def test_no_exploration__has_no_mode_nor_hook(self):
+        exploration = E.NoExploration()
+        self.assertFalse(hasattr(exploration, "_mode"), "should not have `mode`")
+        self.assertFalse(hasattr(exploration, "_hook"), "should not have `_hook`")
+        self.assertIsNone(exploration.hook)
+        self.assertIsNone(exploration.mode)
+
     def test_no_exploration__never_explores(self):
         exploration = E.NoExploration()
         self.assertFalse(exploration.can_explore())
         with self.assertRaisesRegex(
             NotImplementedError, "Perturbation not implemented in NoExploration"
         ):
             exploration.perturbation()
@@ -271,26 +279,14 @@
         do_test_str_and_repr(self, exploration)
 
     @parameterized.expand([("uniform",), ("normal",), ("standard_normal",)])
     def test_greedy_exploration__perturbs(self, method: str):
         exploration = E.GreedyExploration(strength=0.5)
         exploration.perturbation(method)
 
-    def test_epsilon_greedy_exploration__properties_return_right_values(self):
-        epsilon, epsilon_decay_rate = 0.7, 0.75
-        strength, strength_decay_rate = 0.5, 0.75
-        epsilon_scheduler = S.ExponentialScheduler(epsilon, epsilon_decay_rate)
-        strength_scheduler = S.ExponentialScheduler(strength, strength_decay_rate)
-        exploration = E.EpsilonGreedyExploration(
-            epsilon=epsilon_scheduler, strength=strength_scheduler, seed=42
-        )
-        self.assertEqual(exploration.strength, strength)
-        self.assertEqual(exploration.epsilon, epsilon)
-        do_test_str_and_repr(self, exploration)
-
     def test_epsilon_greedy_exploration__never_explores__with_zero_epsilon(self):
         epsilon, epsilon_decay_rate = 0.0, 0.75
         strength, strength_decay_rate = 0.5, 0.75
         epsilon_scheduler = S.ExponentialScheduler(epsilon, epsilon_decay_rate)
         strength_scheduler = S.ExponentialScheduler(strength, strength_decay_rate)
         exploration = E.EpsilonGreedyExploration(
             epsilon=epsilon_scheduler, strength=strength_scheduler, seed=42
@@ -330,20 +326,22 @@
         )
 
         exploration.step()
 
         epsilon_scheduler.step.assert_called_once()
         strength_scheduler.step.assert_called_once()
 
-    def test_stepwise_exploration__has_same_hook_as_base_exploration(self):
-        hook = Mock()
+    def test_stepwise_exploration__has_same_hook_and_mode_as_base_exploration(self):
+        hook, mode = Mock(), Mock()
         base_exploration = Mock()
         base_exploration.hook = hook
+        base_exploration.mode = mode
         exploration = E.StepWiseExploration(base_exploration, 5, 10)
         self.assertIs(exploration.hook, hook)
+        self.assertIs(exploration.mode, mode)
 
     @parameterized.expand([(True,), (False,)])
     def test_stepwise_exploration__turns_base_exploration_into_steps(
         self, stepwise_step: bool
     ):
         base_exploration = E.EpsilonGreedyExploration(0.5, 0.5, seed=0)
         base_exploration.step = Mock()
@@ -558,9 +556,44 @@
         self.assertEqual(strategy.hook, strategy_copy.hook)
         self.assertListEqual(
             [next(strategy._update_cycle) for _ in range(50)],
             [next(strategy_copy._update_cycle) for _ in range(50)],
         )
 
 
+class TestWarmStartStrategy(unittest.TestCase):
+    @parameterized.expand(product((False, True), (False, True)))
+    def test_n_points(self, struct_points: bool, rand_points: bool):
+        ns = np.random.randint(3, 100) if struct_points else 0
+        nr = np.random.randint(3, 100) if rand_points else 0
+        wss = WarmStartStrategy(
+            structured_points=StructuredStartPoints({}, ns) if struct_points else None,
+            random_points=RandomStartPoints({}, nr) if rand_points else None,
+        )
+        self.assertEqual(wss.n_points, ns + nr)
+
+    def test_reset(self):
+        wss = WarmStartStrategy()
+        random_points = Mock()
+        wss.random_points = random_points
+        wss.reset(42)
+        self.assertIsInstance(random_points.np_random, np.random.Generator)
+
+    def test_generate(self):
+        struct_points = Mock()
+        rand_points = Mock()
+        struct_points.__iter__ = lambda self: iter((self,))
+        rand_points.__iter__ = lambda self: iter((self,))
+        wss = WarmStartStrategy(
+            structured_points=struct_points,
+            random_points=rand_points,
+            update_biases_for_random_points=True,
+        )
+        biases = object()
+        out = list(wss.generate(biases=biases))
+        self.assertIs(out[0], struct_points)
+        self.assertIs(out[1], rand_points)
+        rand_points.biases.update.assert_called_once_with(biases)
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mpcrl-1.2.0rc4/tests/test_examples.py` & `mpcrl-1.2.1rc1/tests/test_examples.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import logging
 import os
 import pickle
 import sys
 import unittest
 from operator import neg
 from sys import platform
-from warnings import catch_warnings
+from warnings import filterwarnings
+
+from csnlp.multistart import RandomStartPoint, RandomStartPoints
 
 sys.path.append(os.path.join(os.getcwd(), "examples"))
 
 import casadi as cs
 import numpy as np
 import torch
 from bayesopt import BoTorchOptimizer, CstrEnv, NoisyFilterObservation, get_cstr_mpc
@@ -27,23 +29,24 @@
 from mpcrl import (
     GlobOptLearningAgent,
     LearnableParameter,
     LearnableParametersDict,
     LstdDpgAgent,
     LstdQLearningAgent,
     UpdateStrategy,
+    WarmStartStrategy,
 )
 from mpcrl import exploration as E
 from mpcrl.optim import GradientDescent, NetwonMethod
-from mpcrl.wrappers.agents import Log, RecordUpdates
+from mpcrl.wrappers.agents import Evaluate, Log, RecordUpdates
 from mpcrl.wrappers.envs import MonitorEpisodes
 
 torch.set_default_device("cpu")
 torch.set_default_dtype(torch.float64)
-
+filterwarnings("ignore", "Mpc failure", module="mpcrl")
 
 DATA = loadmat(f"tests/data_test_examples_{platform}.mat", squeeze_me=True)
 
 
 class TestExamples(unittest.TestCase):
     @parameterized.expand([(False,), (True,)])
     def test_q_learning__with_copy_and_pickle(self, use_copy: bool):
@@ -178,42 +181,57 @@
         np.testing.assert_allclose(Jest, DATA["dpg_Jest"], rtol=1e0, atol=1e0)
         np.testing.assert_allclose(Gest, DATA["dpg_Gest"], rtol=1e3, atol=1e3)
         np.testing.assert_allclose(PARS, DATA["dpg_pars"], rtol=1e0, atol=1e0)
 
     @parameterized.expand([(False,), (True,)])
     def test_bayesopt__with_copy_and_pickle(self, use_copy: bool):
         torch.manual_seed(0)
-        env = MonitorEpisodes(TimeLimit(CstrEnv(), max_episode_steps=40))
+        env = MonitorEpisodes(TimeLimit(CstrEnv(4e3), max_episode_steps=10))
         env = TransformReward(env, neg)
         env = NoisyFilterObservation(env, [1, 2])
-        mpc = get_cstr_mpc(env)
+        mpc = get_cstr_mpc(env, horizon=7, multistarts=4, n_jobs=4)
         pars = mpc.parameters
+        Y = mpc.variables["y"].shape
+        U = mpc.variables["u"].shape
         learnable_pars = LearnableParametersDict[cs.SX](
             (
                 LearnableParameter(n, pars[n].shape, (ub + lb) / 2, lb, ub, pars[n])
                 for n, lb, ub in [("narx_weights", -2, 2), ("backoff", 0, 5)]
             )
         )
+        warmstart = WarmStartStrategy(
+            random_points=RandomStartPoints(
+                {
+                    "y": RandomStartPoint("normal", scale=[[1.0], [20.0]], size=Y),
+                    "u": RandomStartPoint("normal", scale=5.0, size=U),
+                },
+                biases={
+                    "y": CstrEnv.x0[[1, 2]].reshape(-1, 1),
+                    "u": sum(CstrEnv.inflow_bound) / 2,
+                },
+                multistarts=4,
+            ),
+        )
         agent = GlobOptLearningAgent(
             mpc=mpc,
             learnable_parameters=learnable_pars,
             optimizer=BoTorchOptimizer(initial_random=2, seed=42),
+            warmstart=warmstart,
         )
         agent = RecordUpdates(agent)
         agent_copy = agent.copy()
         if use_copy:
             agent = agent_copy
 
-        with catch_warnings():
-            J = agent.train(env=env, episodes=5, seed=69, raises=False)
+        J = agent.train(env=env, episodes=6, seed=69, raises=False)
         agent = pickle.loads(pickle.dumps(agent))
 
-        X = np.squeeze(env.observations)
-        U = np.squeeze(env.actions, (2, 3))
-        R = np.squeeze(env.rewards)
+        X = np.squeeze(env.get_wrapper_attr("observations"))
+        U = np.squeeze(env.get_wrapper_attr("actions"), (2, 3))
+        R = np.squeeze(env.get_wrapper_attr("rewards"))
 
         # from scipy.io import savemat
         # DATA.update({"bo_J": J, "bo_X": X, "bo_U": U, "bo_R": R})
         # savemat(f"tests/data_test_examples_{platform}.mat", DATA)
 
         np.testing.assert_allclose(J, DATA["bo_J"], rtol=1e-2, atol=1e-2)
         np.testing.assert_allclose(X, DATA["bo_X"], rtol=1e-2, atol=1e-2)
@@ -227,50 +245,47 @@
             (
                 LearnableParameter(
                     name=name, shape=val.shape, value=val, sym=mpc.parameters[name]
                 )
                 for name, val in mpc.learnable_pars_init.items()
             )
         )
-        agent = Log(
-            RecordUpdates(
-                LstdQLearningAgent(
-                    mpc=mpc,
-                    learnable_parameters=learnable_pars,
-                    discount_factor=mpc.discount_factor,
-                    update_strategy=1,
-                    optimizer=NetwonMethod(learning_rate=5e-2),
-                    hessian_type="approx",
-                    record_td_errors=True,
-                    remove_bounds_on_initial_action=True,
-                )
+        seed = np.random.default_rng(69)
+        agent = Evaluate(
+            Log(
+                RecordUpdates(
+                    LstdQLearningAgent(
+                        mpc=mpc,
+                        learnable_parameters=learnable_pars,
+                        discount_factor=mpc.discount_factor,
+                        update_strategy=1,
+                        optimizer=NetwonMethod(learning_rate=5e-2),
+                        hessian_type="approx",
+                        record_td_errors=True,
+                        remove_bounds_on_initial_action=True,
+                    )
+                ),
+                level=logging.DEBUG,
+                log_frequencies={"on_episode_end": 1},
             ),
-            level=logging.DEBUG,
-            log_frequencies={"on_episode_end": 1},
-        )
-
-        seed = 69
-        env_factory = lambda: MonitorEpisodes(
-            TimeLimit(QLearningOffPolicyLtiSystem(), 100)
+            eval_env=TimeLimit(QLearningOffPolicyLtiSystem(), 100),
+            hook="on_episode_end",
+            frequency=2,
+            n_eval_episodes=2,
+            seed=seed,
         )
-        generate_rollout = get_rollout_generator(env_factory, seed)
+        generate_rollout = get_rollout_generator(rollout_seed=69)
 
         agent_copy = agent.copy()
         if use_copy:
             agent = agent_copy
-        J = agent.train_offpolicy(
-            episode_rollouts=(generate_rollout(n) for n in range(6)),
-            seed=seed,
-            eval_frequency=2,
-            eval_env_factory=env_factory,
-            eval_kwargs={
-                "episodes": 2,
-            },
-            eval_at_start=False,
+        agent.train_offpolicy(
+            episode_rollouts=(generate_rollout(n) for n in range(6)), seed=seed
         )
+        J = np.asarray(agent.eval_returns)
         agent = pickle.loads(pickle.dumps(agent))
 
         parnames = ["V0", "x_lb", "x_ub", "b", "f", "A", "B"]
         PARS = np.concatenate(
             [np.reshape(agent.updates_history[n], -1) for n in parnames]
         )
         TD = np.squeeze(agent.td_errors)
```

### Comparing `mpcrl-1.2.0rc4/tests/test_optim.py` & `mpcrl-1.2.1rc1/tests/test_optim.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/tests/test_util.py` & `mpcrl-1.2.1rc1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.0rc4/tests/test_wrappers.py` & `mpcrl-1.2.1rc1/tests/test_wrappers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import logging
 import os
 import unittest
 from functools import lru_cache
+from itertools import combinations, product
+from random import random
 from typing import Any
 from unittest.mock import Mock, call
 
 import casadi as cs
 import gymnasium as gym
 import numpy as np
 from csnlp import Nlp, scaling
 from csnlp.multistart import StackedMultistartNlp
 from csnlp.wrappers import Mpc, NlpScaling
+from parameterized import parameterized
 
 from mpcrl import (
     Agent,
     LearnableParameter,
     LearnableParametersDict,
     LearningAgent,
     wrappers_agents,
@@ -160,39 +163,40 @@
         self.assertFalse(agent.is_wrapped())
 
         wrapped = wrappers_agents.LearningWrapper(agent)
         self.assertTrue(wrapped.is_wrapped(wrappers_agents.LearningWrapper))
         self.assertFalse(wrapped.is_wrapped(cs.SX))
 
     def test_detach_wrapper(self):
-        agent = mk_agent()
-        wrapped_intermediate = wrappers_agents.RecordUpdates(agent)
-        original_hooks = agent._hooks.copy()
-        wrapped = wrappers_agents.Log(
-            wrapped_intermediate,
-            level=logging.DEBUG,
-            log_frequencies={"on_timestep_end": 1000},
-        )
-        with self.assertRaises(AssertionError):
-            self.assertDictEqual(agent._hooks, original_hooks)
-        wrapped.detach_wrapper()
-        self.assertDictEqual(agent._hooks, original_hooks)
+        cp = lambda d: {k: {k_: id(v_) for k_, v_ in v.items()} for k, v in d.items()}
+        agent_0 = mk_agent()
+        agent_0_hooks = cp(agent_0._hooks)
+        wrapped_1 = wrappers_agents.RecordUpdates(agent_0)
+        wrapped_1_hooks = cp(agent_0._hooks)
+        wrapped_2 = wrappers_agents.Log(
+            wrapped_1, level=logging.DEBUG, log_frequencies={"on_timestep_end": 1000}
+        )
+        wrapped_2_hooks = cp(agent_0._hooks)
+        for d1, d2 in combinations(
+            (agent_0_hooks, wrapped_1_hooks, wrapped_2_hooks), 2
+        ):
+            with self.assertRaises(AssertionError):
+                self.assertDictEqual(d1, d2)
 
-    def test_detach_wrappers(self):
-        agent = mk_agent()
-        original_hooks = agent._hooks.copy()
-        wrapped = wrappers_agents.Log(
-            wrappers_agents.RecordUpdates(agent),
-            level=logging.DEBUG,
-            log_frequencies={"on_timestep_end": 1000},
-        )
-        with self.assertRaises(AssertionError):
-            self.assertDictEqual(agent._hooks, original_hooks)
-        wrapped.detach_wrappers()
-        self.assertDictEqual(agent._hooks, original_hooks)
+        detached_1 = wrapped_2.detach_wrapper()
+        self.assertIs(detached_1, wrapped_1)
+        self.assertDictEqual(cp(agent_0._hooks), wrapped_1_hooks)
+
+        detached_0 = detached_1.detach_wrapper()
+        self.assertIs(detached_0, agent_0)
+        self.assertDictEqual(cp(agent_0._hooks), agent_0_hooks)
+
+        detached_recursive = wrapped_2.detach_wrapper(recursive=True)
+        self.assertIs(detached_recursive, agent_0)
+        self.assertDictEqual(cp(agent_0._hooks), agent_0_hooks)
 
 
 class TestLog(unittest.TestCase):
     def setUp(self):
         self.agent = mk_agent()
         self.env = SimpleEnv()
         self.name = "test_logger"
@@ -347,14 +351,46 @@
         self.assertListEqual(
             [f"p{i}" for i in range(n_params)], list(wrapped.updates_history.keys())
         )
         pars_actual = np.squeeze(list(wrapped.updates_history.values())).T
         np.testing.assert_equal(pars_actual, pars)
 
 
+class TestEvaluate(unittest.TestCase):
+    @parameterized.expand(product((False, True), (False, True)))
+    def test_evaluate__evaluates_with_correct_frequency(
+        self, eval_immediately: bool, fix_seed: bool
+    ):
+        frequency = 10
+        repeats = 2
+        returns = [object() for _ in range(repeats + eval_immediately)]
+        returns_iter = iter(returns)
+        agent = mk_agent()
+        agent.evaluate = Mock(side_effect=lambda *_, **__: next(returns_iter))
+        env = SimpleEnv()
+        wrapped = wrappers_agents.Evaluate(
+            agent,
+            env,
+            "on_episode_end",
+            frequency=frequency,
+            eval_immediately=eval_immediately,
+            fix_seed=fix_seed,
+        )
+
+        n_calls = frequency * repeats
+        n_calls += int(frequency / 2)  # adds some spurious calls
+        [agent.on_episode_end(env, i, random()) for i in range(n_calls)]
+
+        self.assertEqual(agent.evaluate.call_count, repeats + eval_immediately)
+        self.assertListEqual(wrapped.eval_returns, returns)
+        if fix_seed:
+            seeds = (call.args[3] for call in agent.evaluate.call_args_list)
+            self.assertEqual(len(set(seeds)), 1)
+
+
 class TestMonitorEpisodesAndInfos(unittest.TestCase):
     def test__compact_dicts(self):
         act = compact_dicts(
             [
                 {"a": 3, "b": 2},
                 {"b": 3, "c": 2},
                 {"a": 3, "c": 2},
@@ -375,32 +411,46 @@
         env = wrappers_envs.MonitorInfos(SimpleEnv())
         n_episodes = 3
         for _ in range(n_episodes):
             env.reset()
             terminated = truncated = False
             while not (terminated or truncated):
                 _, _, terminated, truncated, _ = env.step(object())
-        self.assertListEqual(list(env.reset_infos), env.INTERNAL_RESET_INFOS)
+        self.assertListEqual(
+            list(env.reset_infos), env.get_wrapper_attr("INTERNAL_RESET_INFOS")
+        )
         self.assertDictEqual(
-            env.finalized_reset_infos(), env.INTERNAL_FINALIZED_RESET_INFOS
+            env.finalized_reset_infos(),
+            env.get_wrapper_attr("INTERNAL_FINALIZED_RESET_INFOS"),
+        )
+        self.assertListEqual(
+            list(env.step_infos), env.get_wrapper_attr("INTERNAL_STEP_INFOS")
         )
-        self.assertListEqual(list(env.step_infos), env.INTERNAL_STEP_INFOS)
         self.assertDictEqual(
-            env.finalized_step_infos(), env.INTERNAL_FINALIZED_STEP_INFOS
+            env.finalized_step_infos(),
+            env.get_wrapper_attr("INTERNAL_FINALIZED_STEP_INFOS"),
         )
 
     def test_monitor_episodes__records_episodes_correctly(self):
         env = wrappers_envs.MonitorEpisodes(SimpleEnv())
         n_episodes = 3
         for _ in range(n_episodes):
             env.reset()
             terminated = truncated = False
             while not (terminated or truncated):
                 _, _, terminated, truncated, _ = env.step(object())
-        np.testing.assert_array_equal(env.observations, env.INTERNAL_OBSERVATIONS)
-        np.testing.assert_array_equal(env.actions, env.INTERNAL_ACTIONS)
-        np.testing.assert_array_equal(env.rewards, env.INTERNAL_REWARDS)
-        self.assertListEqual(list(env.episode_lengths), [env.T_MAX] * n_episodes)
+        np.testing.assert_array_equal(
+            env.observations, env.get_wrapper_attr("INTERNAL_OBSERVATIONS")
+        )
+        np.testing.assert_array_equal(
+            env.actions, env.get_wrapper_attr("INTERNAL_ACTIONS")
+        )
+        np.testing.assert_array_equal(
+            env.rewards, env.get_wrapper_attr("INTERNAL_REWARDS")
+        )
+        self.assertListEqual(
+            list(env.episode_lengths), [env.get_wrapper_attr("T_MAX")] * n_episodes
+        )
 
 
 if __name__ == "__main__":
     unittest.main()
```

