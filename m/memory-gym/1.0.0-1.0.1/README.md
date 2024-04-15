# Comparing `tmp/memory-gym-1.0.0.tar.gz` & `tmp/memory_gym-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory-gym-1.0.0.tar", last modified: Tue Aug  1 12:25:42 2023, max compression
+gzip compressed data, was "memory_gym-1.0.1.tar", last modified: Mon Apr 15 07:31:04 2024, max compression
```

## Comparing `memory-gym-1.0.0.tar` & `memory_gym-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 12:25:42.935213 memory-gym-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-08-01 12:25:26.000000 memory-gym-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    30625 2023-08-01 12:25:42.934212 memory-gym-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    29907 2023-08-01 12:25:26.000000 memory-gym-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 12:25:42.905185 memory-gym-1.0.0/memory_gym/
--rw-rw-rw-   0        0        0     1896 2023-05-12 08:51:33.000000 memory-gym-1.0.0/memory_gym/__init__.py
--rw-rw-rw-   0        0        0    12630 2023-08-01 12:00:30.000000 memory-gym-1.0.0/memory_gym/character_controller.py
--rw-rw-rw-   0        0        0    21705 2023-08-01 12:00:27.000000 memory-gym-1.0.0/memory_gym/endless_mortar_mayhem.py
--rw-rw-rw-   0        0        0    23664 2023-08-01 12:00:27.000000 memory-gym-1.0.0/memory_gym/endless_mystery_path.py
--rw-rw-rw-   0        0        0    25779 2023-08-01 12:16:49.000000 memory-gym-1.0.0/memory_gym/endless_searing_spotlights.py
--rw-rw-rw-   0        0        0      328 2023-05-12 08:47:22.000000 memory-gym-1.0.0/memory_gym/environment.py
--rw-rw-rw-   0        0        0    21491 2023-08-01 12:00:30.000000 memory-gym-1.0.0/memory_gym/mortar_mayhem.py
--rw-rw-rw-   0        0        0    15620 2023-08-01 08:53:49.000000 memory-gym-1.0.0/memory_gym/mortar_mayhem_b.py
--rw-rw-rw-   0        0        0    15624 2023-08-01 12:00:30.000000 memory-gym-1.0.0/memory_gym/mortar_mayhem_b_grid.py
--rw-rw-rw-   0        0        0    21735 2023-08-01 08:54:00.000000 memory-gym-1.0.0/memory_gym/mortar_mayhem_grid.py
--rw-rw-rw-   0        0        0    15298 2023-08-01 12:04:00.000000 memory-gym-1.0.0/memory_gym/mystery_path.py
--rw-rw-rw-   0        0        0    15555 2023-08-01 12:04:08.000000 memory-gym-1.0.0/memory_gym/mystery_path_grid.py
--rw-rw-rw-   0        0        0    36457 2023-08-01 12:00:30.000000 memory-gym-1.0.0/memory_gym/pygame_assets.py
--rw-rw-rw-   0        0        0    28064 2023-08-01 12:00:30.000000 memory-gym-1.0.0/memory_gym/searing_spotlights.py
-drwxrwxrwx   0        0        0        0 2023-08-01 12:25:42.933210 memory-gym-1.0.0/memory_gym.egg-info/
--rw-rw-rw-   0        0        0    30625 2023-08-01 12:25:42.000000 memory-gym-1.0.0/memory_gym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1144 2023-08-01 12:25:42.000000 memory-gym-1.0.0/memory_gym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 12:25:42.000000 memory-gym-1.0.0/memory_gym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      640 2023-08-01 12:25:42.000000 memory-gym-1.0.0/memory_gym.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-08-01 12:25:42.000000 memory-gym-1.0.0/memory_gym.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-01 12:25:42.000000 memory-gym-1.0.0/memory_gym.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 12:25:42.935213 memory-gym-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2274 2023-08-01 12:25:26.000000 memory-gym-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:31:04.347465 memory_gym-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2024-04-15 07:30:51.000000 memory_gym-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    30634 2024-04-15 07:31:04.346465 memory_gym-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    29854 2024-04-15 07:30:51.000000 memory_gym-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 07:31:04.325444 memory_gym-1.0.1/memory_gym/
+-rw-rw-rw-   0        0        0     1896 2023-08-21 08:19:45.000000 memory_gym-1.0.1/memory_gym/__init__.py
+-rw-rw-rw-   0        0        0    12630 2023-08-24 10:26:30.000000 memory_gym-1.0.1/memory_gym/character_controller.py
+-rw-rw-rw-   0        0        0    21682 2024-01-28 12:49:20.000000 memory_gym-1.0.1/memory_gym/endless_mortar_mayhem.py
+-rw-rw-rw-   0        0        0    23640 2024-01-28 12:50:23.000000 memory_gym-1.0.1/memory_gym/endless_mystery_path.py
+-rw-rw-rw-   0        0        0    25755 2024-01-28 12:49:01.000000 memory_gym-1.0.1/memory_gym/endless_searing_spotlights.py
+-rw-rw-rw-   0        0        0      328 2023-08-21 08:19:45.000000 memory_gym-1.0.1/memory_gym/environment.py
+-rw-rw-rw-   0        0        0    21467 2024-01-28 12:50:13.000000 memory_gym-1.0.1/memory_gym/mortar_mayhem.py
+-rw-rw-rw-   0        0        0    15608 2024-01-28 12:49:42.000000 memory_gym-1.0.1/memory_gym/mortar_mayhem_b.py
+-rw-rw-rw-   0        0        0    15611 2024-01-28 12:49:51.000000 memory_gym-1.0.1/memory_gym/mortar_mayhem_b_grid.py
+-rw-rw-rw-   0        0        0    21719 2024-01-28 12:39:18.000000 memory_gym-1.0.1/memory_gym/mortar_mayhem_grid.py
+-rw-rw-rw-   0        0        0    15274 2024-01-28 12:51:19.000000 memory_gym-1.0.1/memory_gym/mystery_path.py
+-rw-rw-rw-   0        0        0    15531 2024-01-28 12:50:07.000000 memory_gym-1.0.1/memory_gym/mystery_path_grid.py
+-rw-rw-rw-   0        0        0    36457 2023-09-23 05:15:45.000000 memory_gym-1.0.1/memory_gym/pygame_assets.py
+-rw-rw-rw-   0        0        0    28043 2024-03-19 07:17:52.000000 memory_gym-1.0.1/memory_gym/searing_spotlights.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:31:04.346465 memory_gym-1.0.1/memory_gym.egg-info/
+-rw-rw-rw-   0        0        0    30634 2024-04-15 07:31:04.000000 memory_gym-1.0.1/memory_gym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1144 2024-04-15 07:31:04.000000 memory_gym-1.0.1/memory_gym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 07:31:04.000000 memory_gym-1.0.1/memory_gym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      640 2024-04-15 07:31:04.000000 memory_gym-1.0.1/memory_gym.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2024-04-15 07:31:04.000000 memory_gym-1.0.1/memory_gym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-15 07:31:04.000000 memory_gym-1.0.1/memory_gym.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 07:31:04.347465 memory_gym-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2274 2024-04-15 07:30:51.000000 memory_gym-1.0.1/setup.py
```

### Comparing `memory-gym-1.0.0/LICENSE` & `memory_gym-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `memory-gym-1.0.0/PKG-INFO` & `memory_gym-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,10 @@
-Metadata-Version: 2.1
-Name: memory-gym
-Version: 1.0.0
-Summary: A gym that contains the memory benchmarks Mortar Mayhem, Mystery Maze and Searing Spotlights
-Home-page: https://github.com/MarcoMeter/drl-memory-gym
-Author: Marco Pleines
-Project-URL: Github, https://github.com/MarcoMeter/drl-memory-gym
-Project-URL: Bug Tracker, https://github.com/MarcoMeter/drl-memory-gym/issues
-Keywords: Deep Reinforcement Learning,gym,POMDP,Imperfect Information,Partial Observation
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[[Paper](https://arxiv.org/abs/2309.17207)] [[Installation](#installation)]  [[Usage](#usage)] [[Mortar Mayhem](#mortar-mayhem)] [[Endless Mortar Mayhem](#endless-mortar-mayhem)] [[Mystery Path](#mystery-path)] [[Endless Mystery Path](#endless-mystery-path)] [[Searing Spotlights](#searing-spotlights)] [[Endless Searing Spotlights](#endless-searing-spotlights)] [[Training](#training)]
 
-[[Paper](https://openreview.net/forum?id=jHc8dCx6DDr)] [[Installation](#installation)]  [[Usage](#usage)] [[Mortar Mayhem](#mortar-mayhem)] [[Endless Mortar Mayhem](#endless-mortar-mayhem)] [[Mystery Path](#mystery-path)] [[Endless Mystery Path](#enndless-mystery-path)] [[Searing Spotlights](#searing-spotlights)] [[Endless Searing Spotlights](#endless-searing-spotlights)] [[Training](#training)]
-
-# Memory Gym: Partially Observable Challenges to Memory-Based Agents in Endless Episodes
+# Memory Gym: Towards Endless Tasks to Benchmark Memory Capabilities of Agents
 
 <table align="center">
   <tr>
     <td></td>
     <td>Endless Mortar Mayhem</td>
     <td>Endless Mystery Path</td>
     <td>Endless Searing Spotlights</td>
@@ -36,30 +20,40 @@
     <td><img src="docs/assets/emm_0_gt.gif" width=180></td>
     <td><img src="docs/assets/emp_0_gt.gif" width=180></td>
     <td><img src="docs/assets/ess_0_gt.gif" width=180></td>
   </tr>
 </table>
 
 
-Memory Gym features the environments **Mortar Mayhem**, **Mystery Path**, and **Searing Spotlights** that are inspired by some mini games of [Pummel Party](http://rebuiltgames.com/). These environments shall benchmark an agent's memory to
-- memorize events across long sequences,
-- generalize,
-- and be robust to noise.
-
-Especially, these environments feature endless task variants. As the agent's policy improves, the task goes on. The traveling game "I packed my bag ..." inspired this dynamic concept, which allows for examining levels of effectinvess instead of just sample efficiency.
+Memory Gym features the environments **Mortar Mayhem**, **Mystery Path**, and **Searing Spotlights** that are inspired by some mini games of [Pummel Party](http://rebuiltgames.com/). These 2D environments benchmark the memory capabilities of agents.
+Especially, these environments feature endless task variants. As the agent's policy improves, the task goes on. The cumulative memory game "I packed my bag ..." inspired this dynamic concept, which allows for examining levels of effectiveness instead of just sample efficiency.
+Interactive videos, based on selected agent behavios, can be found here: https://marcometer.github.io/
 
 ## Citation
 
+Preprint Journal Paper (under review)
+```bibtex
+@misc{pleines2024memory,
+      title={Memory Gym: Towards Endless Tasks to Benchmark Memory Capabilities of Agents}, 
+      author={Marco Pleines and Matthias Pallasch and Frank Zimmer and Mike Preuss},
+      year={2024},
+      eprint={2309.17207},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG}
+}
+```
+
+ICLR Paper
 ```bibtex
 @inproceedings{pleines2023memory,
-title={Memory Gym: Partially Observable Challenges to Memory-Based Agents},
-author={Marco Pleines and Matthias Pallasch and Frank Zimmer and Mike Preuss},
-booktitle={International Conference on Learning Representations},
-year={2023},
-url={https://openreview.net/forum?id=jHc8dCx6DDr}
+      title={Memory Gym: Partially Observable Challenges to Memory-Based Agents},
+      author={Marco Pleines and Matthias Pallasch and Frank Zimmer and Mike Preuss},
+      booktitle={International Conference on Learning Representations},
+      year={2023},
+      url={https://openreview.net/forum?id=jHc8dCx6DDr}
 }
 ```
 
 ## Installation
 
 Major dependencies:
 - gymnasium==0.29.0
@@ -282,15 +276,15 @@
 
 | Parameter                | Default | Explanation                                                                                                     |
 |--------------------------|--------:|-----------------------------------------------------------------------------------------------------------------|
 | max_steps                |     -1 | The maximum number of steps for the agent to play one episode. If smaller than 1, the episode is not affected by this reset parameter.                                                  |
 | steps_per_coin                |     160 | Number of steps that the agent has to collect a newly spawned coin.                                                  |
 | agent_scale              |    0.25 | The dimensions of the agent.                                                                                    |
 | agent_speed              |     3.0 | The speed of the agent.                                                                                         |
-| agent_health             |     10 | The initial health points of the agent.                                                                         |
+| agent_health             |     5 | The initial health points of the agent.                                                                         |
 | agent_visible            |   False | Whether to make the agent permanently visible.                                                                  |
 | sample_agent_position    |    True | Whether to hide or show the goal tile of the generated path.                                                    |
 | num_coins                |     [1] | The number of coins that are spawned. This is a list that the environment samples from.                         |
 | coin_scale               |   0.375 | The scale of the coins.                                                                                         |
 | coins_visible            |   False | Whether to make the coins permanently visible.                                                                  |
 | use_exit                 |    True | Whether to spawn and use the exit task. The exit is accessible by the agent after collecting all coins.         |
 | exit_scale               |     0.0 | The scale of the exit.                                                                                          |
@@ -303,14 +297,16 @@
 | spot_max_speed           | 0.0075  | The maximum speed of the spotlights. The speed is sampled from the range min to max.                            |
 | spot_damage              | 1.0     | Damage per step while the agent is spotted by one spotlight.                                                    |
 | light_dim_off_duration   | 6       | The number of steps to dim off the global light.                                                                |
 | light_threshold          | 255     | The threshold for dimming the global light. A value of 255 indicates that the light will dimmed of completely.  |
 | visual_feedback          | True    | Whether to render the tiled background red if the agent is spotted.                                             |
 | black_background         | False   | Whether to render the environments background black, while the spotlights are rendered as white circumferences. |
 | hide_chessboard          | False   | Whether to hide the chessboard background. This renders the background of the environment white.                           |
+| show_last_action         | True    | Whether to encode and render the previouss action to the visual observation.                                    |
+| show_last_positive_reward | True   | Whether to render if the agent received a positive reward on the previous step.                                 |
 | reward_inside_spotlight  | 0.0     | What reward to signal for each step while being inside a spotlight.                                             |
 | reward_outside_spotlight | 0.0     | What reward to signal for each step while being outside of a spotlight.                                         |
 | reward_death             | 0.0     | What reward to signal upon losing all health points.                                                            |
 | reward_coin              | 0.25    | What reward to signal upon collecting one coin.                                                                 |
 
 ## Endless Searing Spotlights
 
@@ -319,43 +315,38 @@
 ### Reset Parameters
 
 | Parameter                | Default | Explanation                                                                                                     |
 |--------------------------|--------:|-----------------------------------------------------------------------------------------------------------------|
 | max_steps                |     -1 | The maximum number of steps for the agent to play one episode.                                                  |
 | agent_scale              |    0.25 | The dimensions of the agent.                                                                                    |
 | agent_speed              |     3.0 | The speed of the agent.                                                                                         |
-| agent_health             |     100 | The initial health points of the agent.                                                                         |
+| agent_health             |     10 | The initial health points of the agent.                                                                         |
 | agent_visible            |   False | Whether to make the agent permanently visible.                                                                  |
 | sample_agent_position    |    True | Whether to hide or show the goal tile of the generated path.                                                    |
-| num_coins                |     [1] | The number of coins that are spawned. This is a list that the environment samples from.                         |
+| coin_show_duration       |     6 | How many steps to make the coin visible to the agent unill its hidden behind the dark.                         |
 | coin_scale               |   0.375 | The scale of the coins.                                                                                         |
 | coins_visible            |   False | Whether to make the coins permanently visible.                                                                  |
-| use_exit                 |    True | Whether to spawn and use the exit task. The exit is accessible by the agent after collecting all coins.         |
-| exit_scale               |     0.0 | The scale of the exit.                                                                                          |
-| exit_visible             | False   | Whether to make the exit permanently visible.                                                                   |
-| initial_spawns           | 4       | The number of spotlights that are initially spawned.                                                            |
-| num_spawns               | 30      | The number of spotlights that are to be spawned.                                                                |
-| initial_spawn_interval   | 30      | The number of steps until the next spotlight is spawned.                                                        |
-| spawn_interval_threshold | 10      | The spawn interval is decayed until reaching this lower threshold.                                              |
-| spawn_interval_decay     | 0.95    | The decay rate of the spotlight spawn interval.                                                                 |
+| steps_per_coin            |   160 | Time budget to collect a single coin.                                                                  |
+| initial_spawns           | 3       | The number of spotlights that are initially spawned.                                                            |
+| spawn_interval   | 50      | The number of steps until the next spotlight is spawned.                                                        |
 | spot_min_radius          | 7.5     | The minimum radius of the spotlights. The radius is sampled from the range min to max.                          |
 | spot_max_radius          | 13.75   | The maximum radius of the spotlights. The radius is sampled from the range min to max.                          |
 | spot_min_speed           | 0.0025  | The minimum speed of the spotlights. The speed is sampled from the range min to max.                            |
 | spot_max_speed           | 0.0075  | The maximum speed of the spotlights. The speed is sampled from the range min to max.                            |
 | spot_damage              | 1.0     | Damage per step while the agent is spotted by one spotlight.                                                    |
 | light_dim_off_duration   | 6       | The number of steps to dim off the global light.                                                                |
 | light_threshold          | 255     | The threshold for dimming the global light. A value of 255 indicates that the light will dimmed of completely.  |
 | visual_feedback          | True    | Whether to render the tiled background red if the agent is spotted.                                             |
 | black_background         | False   | Whether to render the environments background black, while the spotlights are rendered as white circumferences. |
 | hide_chessboard          | False   | Whether to hide the chessboard background. This renders the background of the environment white.                           |
+| show_last_action         | True    | Whether to encode and render the previouss action to the visual observation.                                    |
+| show_last_positive_reward | True   | Whether to render if the agent received a positive reward on the previous step.                                 |
 | reward_inside_spotlight  | 0.0     | What reward to signal for each step while being inside a spotlight.                                             |
 | reward_outside_spotlight | 0.0     | What reward to signal for each step while being outside of a spotlight.                                         |
 | reward_death             | 0.0     | What reward to signal upon losing all health points.                                                            |
-| reward_exit              | 1.0     | What reward to signal after successfully using the exit.                                                        |
-| reward_max_steps         | 0.0     | What reward to signal if max steps is reached.                                                                  |
 | reward_coin              | 0.25    | What reward to signal upon collecting one coin.                                                                 |
 
 ## Training
 
 Baseline results are avaible via these repositories.
 
 [Recurrence + PPO](https://github.com/MarcoMeter/recurrent-ppo-truncated-bptt)
```

#### html2text {}

```diff
@@ -1,37 +1,33 @@
-Metadata-Version: 2.1 Name: memory-gym Version: 1.0.0 Summary: A gym that
-contains the memory benchmarks Mortar Mayhem, Mystery Maze and Searing
-Spotlights Home-page: https://github.com/MarcoMeter/drl-memory-gym Author:
-Marco Pleines Project-URL: Github, https://github.com/MarcoMeter/drl-memory-gym
-Project-URL: Bug Tracker, https://github.com/MarcoMeter/drl-memory-gym/issues
-Keywords: Deep Reinforcement Learning,gym,POMDP,Imperfect Information,Partial
-Observation Classifier: Programming Language :: Python :: 3 Classifier: License
-:: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE [[Paper](https://openreview.net/forum?id=jHc8dCx6DDr)] [[Installation]
-(#installation)] [[Usage](#usage)] [[Mortar Mayhem](#mortar-mayhem)] [[Endless
-Mortar Mayhem](#endless-mortar-mayhem)] [[Mystery Path](#mystery-path)] [
-[Endless Mystery Path](#enndless-mystery-path)] [[Searing Spotlights](#searing-
-spotlights)] [[Endless Searing Spotlights](#endless-searing-spotlights)] [
-[Training](#training)] # Memory Gym: Partially Observable Challenges to Memory-
-Based Agents in Endless Episodes
+[[Paper](https://arxiv.org/abs/2309.17207)] [[Installation](#installation)] [
+[Usage](#usage)] [[Mortar Mayhem](#mortar-mayhem)] [[Endless Mortar Mayhem]
+(#endless-mortar-mayhem)] [[Mystery Path](#mystery-path)] [[Endless Mystery
+Path](#endless-mystery-path)] [[Searing Spotlights](#searing-spotlights)] [
+[Endless Searing Spotlights](#endless-searing-spotlights)] [[Training]
+(#training)] # Memory Gym: Towards Endless Tasks to Benchmark Memory
+Capabilities of Agents
                    Endless Mortar Mayhem Endless Mystery Path Endless Searing
                                                               Spotlights
  Agent Observation [docs/assets/         [docs/assets/        [docs/assets/
                    emm_0.gif]            emp_0.gif]           ess_0.gif]
  Ground Truth      [docs/assets/         [docs/assets/        [docs/assets/
                    emm_0_gt.gif]         emp_0_gt.gif]        ess_0_gt.gif]
 Memory Gym features the environments **Mortar Mayhem**, **Mystery Path**, and
 **Searing Spotlights** that are inspired by some mini games of [Pummel Party]
-(http://rebuiltgames.com/). These environments shall benchmark an agent's
-memory to - memorize events across long sequences, - generalize, - and be
-robust to noise. Especially, these environments feature endless task variants.
-As the agent's policy improves, the task goes on. The traveling game "I packed
-my bag ..." inspired this dynamic concept, which allows for examining levels of
-effectinvess instead of just sample efficiency. ## Citation ```bibtex
+(http://rebuiltgames.com/). These 2D environments benchmark the memory
+capabilities of agents. Especially, these environments feature endless task
+variants. As the agent's policy improves, the task goes on. The cumulative
+memory game "I packed my bag ..." inspired this dynamic concept, which allows
+for examining levels of effectiveness instead of just sample efficiency.
+Interactive videos, based on selected agent behavios, can be found here: https:
+//marcometer.github.io/ ## Citation Preprint Journal Paper (under review)
+```bibtex @misc{pleines2024memory, title={Memory Gym: Towards Endless Tasks to
+Benchmark Memory Capabilities of Agents}, author={Marco Pleines and Matthias
+Pallasch and Frank Zimmer and Mike Preuss}, year={2024}, eprint={2309.17207},
+archivePrefix={arXiv}, primaryClass={cs.LG} } ``` ICLR Paper ```bibtex
 @inproceedings{pleines2023memory, title={Memory Gym: Partially Observable
 Challenges to Memory-Based Agents}, author={Marco Pleines and Matthias Pallasch
 and Frank Zimmer and Mike Preuss}, booktitle={International Conference on
 Learning Representations}, year={2023}, url={https://openreview.net/
 forum?id=jHc8dCx6DDr} } ``` ## Installation Major dependencies: -
 gymnasium==0.29.0 - PyGame==2.4.0 ```console conda create -n memory-gym
 python=3.11 --yes conda activate memory-gym pip install memory-gym ``` or
@@ -186,15 +182,15 @@
 docs/assets/spots.jpg) ### Reset Parameters | Parameter | Default | Explanation
 | |--------------------------|--------:|---------------------------------------
 --------------------------------------------------------------------------| |
 max_steps | -1 | The maximum number of steps for the agent to play one episode.
 If smaller than 1, the episode is not affected by this reset parameter. | |
 steps_per_coin | 160 | Number of steps that the agent has to collect a newly
 spawned coin. | | agent_scale | 0.25 | The dimensions of the agent. | |
-agent_speed | 3.0 | The speed of the agent. | | agent_health | 10 | The initial
+agent_speed | 3.0 | The speed of the agent. | | agent_health | 5 | The initial
 health points of the agent. | | agent_visible | False | Whether to make the
 agent permanently visible. | | sample_agent_position | True | Whether to hide
 or show the goal tile of the generated path. | | num_coins | [1] | The number
 of coins that are spawned. This is a list that the environment samples from. |
 | coin_scale | 0.375 | The scale of the coins. | | coins_visible | False |
 Whether to make the coins permanently visible. | | use_exit | True | Whether to
 spawn and use the exit task. The exit is accessible by the agent after
@@ -213,64 +209,62 @@
 global light. | | light_threshold | 255 | The threshold for dimming the global
 light. A value of 255 indicates that the light will dimmed of completely. | |
 visual_feedback | True | Whether to render the tiled background red if the
 agent is spotted. | | black_background | False | Whether to render the
 environments background black, while the spotlights are rendered as white
 circumferences. | | hide_chessboard | False | Whether to hide the chessboard
 background. This renders the background of the environment white. | |
+show_last_action | True | Whether to encode and render the previouss action to
+the visual observation. | | show_last_positive_reward | True | Whether to
+render if the agent received a positive reward on the previous step. | |
 reward_inside_spotlight | 0.0 | What reward to signal for each step while being
 inside a spotlight. | | reward_outside_spotlight | 0.0 | What reward to signal
 for each step while being outside of a spotlight. | | reward_death | 0.0 | What
 reward to signal upon losing all health points. | | reward_coin | 0.25 | What
 reward to signal upon collecting one coin. | ## Endless Searing Spotlights
 Endless Searing Spotlights solely revolves around a coin collection task, with
 no consideration of an exit task leading to episode termination. Upon
 collecting the only coin present, a new one is immediately spawned. The agent
 operates under a limited time budget to collect the newly spawned coin. ###
 Reset Parameters | Parameter | Default | Explanation | |-----------------------
 ---|--------:|-----------------------------------------------------------------
 ------------------------------------------------| | max_steps | -1 | The
 maximum number of steps for the agent to play one episode. | | agent_scale |
 0.25 | The dimensions of the agent. | | agent_speed | 3.0 | The speed of the
-agent. | | agent_health | 100 | The initial health points of the agent. | |
+agent. | | agent_health | 10 | The initial health points of the agent. | |
 agent_visible | False | Whether to make the agent permanently visible. | |
 sample_agent_position | True | Whether to hide or show the goal tile of the
-generated path. | | num_coins | [1] | The number of coins that are spawned.
-This is a list that the environment samples from. | | coin_scale | 0.375 | The
-scale of the coins. | | coins_visible | False | Whether to make the coins
-permanently visible. | | use_exit | True | Whether to spawn and use the exit
-task. The exit is accessible by the agent after collecting all coins. | |
-exit_scale | 0.0 | The scale of the exit. | | exit_visible | False | Whether to
-make the exit permanently visible. | | initial_spawns | 4 | The number of
-spotlights that are initially spawned. | | num_spawns | 30 | The number of
-spotlights that are to be spawned. | | initial_spawn_interval | 30 | The number
-of steps until the next spotlight is spawned. | | spawn_interval_threshold | 10
-| The spawn interval is decayed until reaching this lower threshold. | |
-spawn_interval_decay | 0.95 | The decay rate of the spotlight spawn interval. |
-| spot_min_radius | 7.5 | The minimum radius of the spotlights. The radius is
-sampled from the range min to max. | | spot_max_radius | 13.75 | The maximum
-radius of the spotlights. The radius is sampled from the range min to max. | |
-spot_min_speed | 0.0025 | The minimum speed of the spotlights. The speed is
-sampled from the range min to max. | | spot_max_speed | 0.0075 | The maximum
-speed of the spotlights. The speed is sampled from the range min to max. | |
-spot_damage | 1.0 | Damage per step while the agent is spotted by one
+generated path. | | coin_show_duration | 6 | How many steps to make the coin
+visible to the agent unill its hidden behind the dark. | | coin_scale | 0.375 |
+The scale of the coins. | | coins_visible | False | Whether to make the coins
+permanently visible. | | steps_per_coin | 160 | Time budget to collect a single
+coin. | | initial_spawns | 3 | The number of spotlights that are initially
+spawned. | | spawn_interval | 50 | The number of steps until the next spotlight
+is spawned. | | spot_min_radius | 7.5 | The minimum radius of the spotlights.
+The radius is sampled from the range min to max. | | spot_max_radius | 13.75 |
+The maximum radius of the spotlights. The radius is sampled from the range min
+to max. | | spot_min_speed | 0.0025 | The minimum speed of the spotlights. The
+speed is sampled from the range min to max. | | spot_max_speed | 0.0075 | The
+maximum speed of the spotlights. The speed is sampled from the range min to
+max. | | spot_damage | 1.0 | Damage per step while the agent is spotted by one
 spotlight. | | light_dim_off_duration | 6 | The number of steps to dim off the
 global light. | | light_threshold | 255 | The threshold for dimming the global
 light. A value of 255 indicates that the light will dimmed of completely. | |
 visual_feedback | True | Whether to render the tiled background red if the
 agent is spotted. | | black_background | False | Whether to render the
 environments background black, while the spotlights are rendered as white
 circumferences. | | hide_chessboard | False | Whether to hide the chessboard
 background. This renders the background of the environment white. | |
+show_last_action | True | Whether to encode and render the previouss action to
+the visual observation. | | show_last_positive_reward | True | Whether to
+render if the agent received a positive reward on the previous step. | |
 reward_inside_spotlight | 0.0 | What reward to signal for each step while being
 inside a spotlight. | | reward_outside_spotlight | 0.0 | What reward to signal
 for each step while being outside of a spotlight. | | reward_death | 0.0 | What
-reward to signal upon losing all health points. | | reward_exit | 1.0 | What
-reward to signal after successfully using the exit. | | reward_max_steps | 0.0
-| What reward to signal if max steps is reached. | | reward_coin | 0.25 | What
+reward to signal upon losing all health points. | | reward_coin | 0.25 | What
 reward to signal upon collecting one coin. | ## Training Baseline results are
 avaible via these repositories. [Recurrence + PPO](https://github.com/
 MarcoMeter/recurrent-ppo-truncated-bptt) [TransformerXL + PPO](https://
 github.com/MarcoMeter/episodic-transformer-memory-ppo) ## Changelog v1.0.0
 Improvements - All environment concepts are extrapolated to endless episodes! -
 Endless Mortar Mayhem - Endless Mystery Path - Endless Searing Spotlights -
 Improved simulation speed by using already rotated sprites and not rotating the
```

### Comparing `memory-gym-1.0.0/README.md` & `memory_gym-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,28 @@
-[[Paper](https://openreview.net/forum?id=jHc8dCx6DDr)] [[Installation](#installation)]  [[Usage](#usage)] [[Mortar Mayhem](#mortar-mayhem)] [[Endless Mortar Mayhem](#endless-mortar-mayhem)] [[Mystery Path](#mystery-path)] [[Endless Mystery Path](#enndless-mystery-path)] [[Searing Spotlights](#searing-spotlights)] [[Endless Searing Spotlights](#endless-searing-spotlights)] [[Training](#training)]
+Metadata-Version: 2.1
+Name: memory-gym
+Version: 1.0.1
+Summary: A gym that contains the memory benchmarks Mortar Mayhem, Mystery Maze and Searing Spotlights
+Home-page: https://github.com/MarcoMeter/drl-memory-gym
+Author: Marco Pleines
+Project-URL: Github, https://github.com/MarcoMeter/drl-memory-gym
+Project-URL: Bug Tracker, https://github.com/MarcoMeter/drl-memory-gym/issues
+Keywords: Deep Reinforcement Learning,gym,POMDP,Imperfect Information,Partial Observation
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: gymnasium==0.29.0
+Requires-Dist: pygame==2.4.0
 
-# Memory Gym: Partially Observable Challenges to Memory-Based Agents in Endless Episodes
+[[Paper](https://arxiv.org/abs/2309.17207)] [[Installation](#installation)]  [[Usage](#usage)] [[Mortar Mayhem](#mortar-mayhem)] [[Endless Mortar Mayhem](#endless-mortar-mayhem)] [[Mystery Path](#mystery-path)] [[Endless Mystery Path](#endless-mystery-path)] [[Searing Spotlights](#searing-spotlights)] [[Endless Searing Spotlights](#endless-searing-spotlights)] [[Training](#training)]
+
+# Memory Gym: Towards Endless Tasks to Benchmark Memory Capabilities of Agents
 
 <table align="center">
   <tr>
     <td></td>
     <td>Endless Mortar Mayhem</td>
     <td>Endless Mystery Path</td>
     <td>Endless Searing Spotlights</td>
@@ -20,30 +38,40 @@
     <td><img src="docs/assets/emm_0_gt.gif" width=180></td>
     <td><img src="docs/assets/emp_0_gt.gif" width=180></td>
     <td><img src="docs/assets/ess_0_gt.gif" width=180></td>
   </tr>
 </table>
 
 
-Memory Gym features the environments **Mortar Mayhem**, **Mystery Path**, and **Searing Spotlights** that are inspired by some mini games of [Pummel Party](http://rebuiltgames.com/). These environments shall benchmark an agent's memory to
-- memorize events across long sequences,
-- generalize,
-- and be robust to noise.
-
-Especially, these environments feature endless task variants. As the agent's policy improves, the task goes on. The traveling game "I packed my bag ..." inspired this dynamic concept, which allows for examining levels of effectinvess instead of just sample efficiency.
+Memory Gym features the environments **Mortar Mayhem**, **Mystery Path**, and **Searing Spotlights** that are inspired by some mini games of [Pummel Party](http://rebuiltgames.com/). These 2D environments benchmark the memory capabilities of agents.
+Especially, these environments feature endless task variants. As the agent's policy improves, the task goes on. The cumulative memory game "I packed my bag ..." inspired this dynamic concept, which allows for examining levels of effectiveness instead of just sample efficiency.
+Interactive videos, based on selected agent behavios, can be found here: https://marcometer.github.io/
 
 ## Citation
 
+Preprint Journal Paper (under review)
+```bibtex
+@misc{pleines2024memory,
+      title={Memory Gym: Towards Endless Tasks to Benchmark Memory Capabilities of Agents}, 
+      author={Marco Pleines and Matthias Pallasch and Frank Zimmer and Mike Preuss},
+      year={2024},
+      eprint={2309.17207},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG}
+}
+```
+
+ICLR Paper
 ```bibtex
 @inproceedings{pleines2023memory,
-title={Memory Gym: Partially Observable Challenges to Memory-Based Agents},
-author={Marco Pleines and Matthias Pallasch and Frank Zimmer and Mike Preuss},
-booktitle={International Conference on Learning Representations},
-year={2023},
-url={https://openreview.net/forum?id=jHc8dCx6DDr}
+      title={Memory Gym: Partially Observable Challenges to Memory-Based Agents},
+      author={Marco Pleines and Matthias Pallasch and Frank Zimmer and Mike Preuss},
+      booktitle={International Conference on Learning Representations},
+      year={2023},
+      url={https://openreview.net/forum?id=jHc8dCx6DDr}
 }
 ```
 
 ## Installation
 
 Major dependencies:
 - gymnasium==0.29.0
@@ -266,15 +294,15 @@
 
 | Parameter                | Default | Explanation                                                                                                     |
 |--------------------------|--------:|-----------------------------------------------------------------------------------------------------------------|
 | max_steps                |     -1 | The maximum number of steps for the agent to play one episode. If smaller than 1, the episode is not affected by this reset parameter.                                                  |
 | steps_per_coin                |     160 | Number of steps that the agent has to collect a newly spawned coin.                                                  |
 | agent_scale              |    0.25 | The dimensions of the agent.                                                                                    |
 | agent_speed              |     3.0 | The speed of the agent.                                                                                         |
-| agent_health             |     10 | The initial health points of the agent.                                                                         |
+| agent_health             |     5 | The initial health points of the agent.                                                                         |
 | agent_visible            |   False | Whether to make the agent permanently visible.                                                                  |
 | sample_agent_position    |    True | Whether to hide or show the goal tile of the generated path.                                                    |
 | num_coins                |     [1] | The number of coins that are spawned. This is a list that the environment samples from.                         |
 | coin_scale               |   0.375 | The scale of the coins.                                                                                         |
 | coins_visible            |   False | Whether to make the coins permanently visible.                                                                  |
 | use_exit                 |    True | Whether to spawn and use the exit task. The exit is accessible by the agent after collecting all coins.         |
 | exit_scale               |     0.0 | The scale of the exit.                                                                                          |
@@ -287,14 +315,16 @@
 | spot_max_speed           | 0.0075  | The maximum speed of the spotlights. The speed is sampled from the range min to max.                            |
 | spot_damage              | 1.0     | Damage per step while the agent is spotted by one spotlight.                                                    |
 | light_dim_off_duration   | 6       | The number of steps to dim off the global light.                                                                |
 | light_threshold          | 255     | The threshold for dimming the global light. A value of 255 indicates that the light will dimmed of completely.  |
 | visual_feedback          | True    | Whether to render the tiled background red if the agent is spotted.                                             |
 | black_background         | False   | Whether to render the environments background black, while the spotlights are rendered as white circumferences. |
 | hide_chessboard          | False   | Whether to hide the chessboard background. This renders the background of the environment white.                           |
+| show_last_action         | True    | Whether to encode and render the previouss action to the visual observation.                                    |
+| show_last_positive_reward | True   | Whether to render if the agent received a positive reward on the previous step.                                 |
 | reward_inside_spotlight  | 0.0     | What reward to signal for each step while being inside a spotlight.                                             |
 | reward_outside_spotlight | 0.0     | What reward to signal for each step while being outside of a spotlight.                                         |
 | reward_death             | 0.0     | What reward to signal upon losing all health points.                                                            |
 | reward_coin              | 0.25    | What reward to signal upon collecting one coin.                                                                 |
 
 ## Endless Searing Spotlights
 
@@ -303,43 +333,38 @@
 ### Reset Parameters
 
 | Parameter                | Default | Explanation                                                                                                     |
 |--------------------------|--------:|-----------------------------------------------------------------------------------------------------------------|
 | max_steps                |     -1 | The maximum number of steps for the agent to play one episode.                                                  |
 | agent_scale              |    0.25 | The dimensions of the agent.                                                                                    |
 | agent_speed              |     3.0 | The speed of the agent.                                                                                         |
-| agent_health             |     100 | The initial health points of the agent.                                                                         |
+| agent_health             |     10 | The initial health points of the agent.                                                                         |
 | agent_visible            |   False | Whether to make the agent permanently visible.                                                                  |
 | sample_agent_position    |    True | Whether to hide or show the goal tile of the generated path.                                                    |
-| num_coins                |     [1] | The number of coins that are spawned. This is a list that the environment samples from.                         |
+| coin_show_duration       |     6 | How many steps to make the coin visible to the agent unill its hidden behind the dark.                         |
 | coin_scale               |   0.375 | The scale of the coins.                                                                                         |
 | coins_visible            |   False | Whether to make the coins permanently visible.                                                                  |
-| use_exit                 |    True | Whether to spawn and use the exit task. The exit is accessible by the agent after collecting all coins.         |
-| exit_scale               |     0.0 | The scale of the exit.                                                                                          |
-| exit_visible             | False   | Whether to make the exit permanently visible.                                                                   |
-| initial_spawns           | 4       | The number of spotlights that are initially spawned.                                                            |
-| num_spawns               | 30      | The number of spotlights that are to be spawned.                                                                |
-| initial_spawn_interval   | 30      | The number of steps until the next spotlight is spawned.                                                        |
-| spawn_interval_threshold | 10      | The spawn interval is decayed until reaching this lower threshold.                                              |
-| spawn_interval_decay     | 0.95    | The decay rate of the spotlight spawn interval.                                                                 |
+| steps_per_coin            |   160 | Time budget to collect a single coin.                                                                  |
+| initial_spawns           | 3       | The number of spotlights that are initially spawned.                                                            |
+| spawn_interval   | 50      | The number of steps until the next spotlight is spawned.                                                        |
 | spot_min_radius          | 7.5     | The minimum radius of the spotlights. The radius is sampled from the range min to max.                          |
 | spot_max_radius          | 13.75   | The maximum radius of the spotlights. The radius is sampled from the range min to max.                          |
 | spot_min_speed           | 0.0025  | The minimum speed of the spotlights. The speed is sampled from the range min to max.                            |
 | spot_max_speed           | 0.0075  | The maximum speed of the spotlights. The speed is sampled from the range min to max.                            |
 | spot_damage              | 1.0     | Damage per step while the agent is spotted by one spotlight.                                                    |
 | light_dim_off_duration   | 6       | The number of steps to dim off the global light.                                                                |
 | light_threshold          | 255     | The threshold for dimming the global light. A value of 255 indicates that the light will dimmed of completely.  |
 | visual_feedback          | True    | Whether to render the tiled background red if the agent is spotted.                                             |
 | black_background         | False   | Whether to render the environments background black, while the spotlights are rendered as white circumferences. |
 | hide_chessboard          | False   | Whether to hide the chessboard background. This renders the background of the environment white.                           |
+| show_last_action         | True    | Whether to encode and render the previouss action to the visual observation.                                    |
+| show_last_positive_reward | True   | Whether to render if the agent received a positive reward on the previous step.                                 |
 | reward_inside_spotlight  | 0.0     | What reward to signal for each step while being inside a spotlight.                                             |
 | reward_outside_spotlight | 0.0     | What reward to signal for each step while being outside of a spotlight.                                         |
 | reward_death             | 0.0     | What reward to signal upon losing all health points.                                                            |
-| reward_exit              | 1.0     | What reward to signal after successfully using the exit.                                                        |
-| reward_max_steps         | 0.0     | What reward to signal if max steps is reached.                                                                  |
 | reward_coin              | 0.25    | What reward to signal upon collecting one coin.                                                                 |
 
 ## Training
 
 Baseline results are avaible via these repositories.
 
 [Recurrence + PPO](https://github.com/MarcoMeter/recurrent-ppo-truncated-bptt)
@@ -360,8 +385,8 @@
 - All endless environments feature a ground truth space. As specified by this space ground truth information is added to the info dictionary
 - Searing Spotlights may also visualize whether a positive reward was signaled on the previous frame
 
 Breaking Changes
 - Refactored the info key "exit_success" in Searing Spotlights to "success"
 
 Bug Fixes
-- Fixed the speed of character controller, because moving downwards was slower than moving upwards due to float truncation
+- Fixed the speed of character controller, because moving downwards was slower than moving upwards due to float truncation
```

#### html2text {}

```diff
@@ -1,28 +1,42 @@
-[[Paper](https://openreview.net/forum?id=jHc8dCx6DDr)] [[Installation]
-(#installation)] [[Usage](#usage)] [[Mortar Mayhem](#mortar-mayhem)] [[Endless
-Mortar Mayhem](#endless-mortar-mayhem)] [[Mystery Path](#mystery-path)] [
-[Endless Mystery Path](#enndless-mystery-path)] [[Searing Spotlights](#searing-
-spotlights)] [[Endless Searing Spotlights](#endless-searing-spotlights)] [
-[Training](#training)] # Memory Gym: Partially Observable Challenges to Memory-
-Based Agents in Endless Episodes
+Metadata-Version: 2.1 Name: memory-gym Version: 1.0.1 Summary: A gym that
+contains the memory benchmarks Mortar Mayhem, Mystery Maze and Searing
+Spotlights Home-page: https://github.com/MarcoMeter/drl-memory-gym Author:
+Marco Pleines Project-URL: Github, https://github.com/MarcoMeter/drl-memory-gym
+Project-URL: Bug Tracker, https://github.com/MarcoMeter/drl-memory-gym/issues
+Keywords: Deep Reinforcement Learning,gym,POMDP,Imperfect Information,Partial
+Observation Classifier: Programming Language :: Python :: 3 Classifier: License
+:: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: gymnasium==0.29.0 Requires-Dist: pygame==2.4.0 [[Paper]
+(https://arxiv.org/abs/2309.17207)] [[Installation](#installation)] [[Usage]
+(#usage)] [[Mortar Mayhem](#mortar-mayhem)] [[Endless Mortar Mayhem](#endless-
+mortar-mayhem)] [[Mystery Path](#mystery-path)] [[Endless Mystery Path]
+(#endless-mystery-path)] [[Searing Spotlights](#searing-spotlights)] [[Endless
+Searing Spotlights](#endless-searing-spotlights)] [[Training](#training)] #
+Memory Gym: Towards Endless Tasks to Benchmark Memory Capabilities of Agents
                    Endless Mortar Mayhem Endless Mystery Path Endless Searing
                                                               Spotlights
  Agent Observation [docs/assets/         [docs/assets/        [docs/assets/
                    emm_0.gif]            emp_0.gif]           ess_0.gif]
  Ground Truth      [docs/assets/         [docs/assets/        [docs/assets/
                    emm_0_gt.gif]         emp_0_gt.gif]        ess_0_gt.gif]
 Memory Gym features the environments **Mortar Mayhem**, **Mystery Path**, and
 **Searing Spotlights** that are inspired by some mini games of [Pummel Party]
-(http://rebuiltgames.com/). These environments shall benchmark an agent's
-memory to - memorize events across long sequences, - generalize, - and be
-robust to noise. Especially, these environments feature endless task variants.
-As the agent's policy improves, the task goes on. The traveling game "I packed
-my bag ..." inspired this dynamic concept, which allows for examining levels of
-effectinvess instead of just sample efficiency. ## Citation ```bibtex
+(http://rebuiltgames.com/). These 2D environments benchmark the memory
+capabilities of agents. Especially, these environments feature endless task
+variants. As the agent's policy improves, the task goes on. The cumulative
+memory game "I packed my bag ..." inspired this dynamic concept, which allows
+for examining levels of effectiveness instead of just sample efficiency.
+Interactive videos, based on selected agent behavios, can be found here: https:
+//marcometer.github.io/ ## Citation Preprint Journal Paper (under review)
+```bibtex @misc{pleines2024memory, title={Memory Gym: Towards Endless Tasks to
+Benchmark Memory Capabilities of Agents}, author={Marco Pleines and Matthias
+Pallasch and Frank Zimmer and Mike Preuss}, year={2024}, eprint={2309.17207},
+archivePrefix={arXiv}, primaryClass={cs.LG} } ``` ICLR Paper ```bibtex
 @inproceedings{pleines2023memory, title={Memory Gym: Partially Observable
 Challenges to Memory-Based Agents}, author={Marco Pleines and Matthias Pallasch
 and Frank Zimmer and Mike Preuss}, booktitle={International Conference on
 Learning Representations}, year={2023}, url={https://openreview.net/
 forum?id=jHc8dCx6DDr} } ``` ## Installation Major dependencies: -
 gymnasium==0.29.0 - PyGame==2.4.0 ```console conda create -n memory-gym
 python=3.11 --yes conda activate memory-gym pip install memory-gym ``` or
@@ -177,15 +191,15 @@
 docs/assets/spots.jpg) ### Reset Parameters | Parameter | Default | Explanation
 | |--------------------------|--------:|---------------------------------------
 --------------------------------------------------------------------------| |
 max_steps | -1 | The maximum number of steps for the agent to play one episode.
 If smaller than 1, the episode is not affected by this reset parameter. | |
 steps_per_coin | 160 | Number of steps that the agent has to collect a newly
 spawned coin. | | agent_scale | 0.25 | The dimensions of the agent. | |
-agent_speed | 3.0 | The speed of the agent. | | agent_health | 10 | The initial
+agent_speed | 3.0 | The speed of the agent. | | agent_health | 5 | The initial
 health points of the agent. | | agent_visible | False | Whether to make the
 agent permanently visible. | | sample_agent_position | True | Whether to hide
 or show the goal tile of the generated path. | | num_coins | [1] | The number
 of coins that are spawned. This is a list that the environment samples from. |
 | coin_scale | 0.375 | The scale of the coins. | | coins_visible | False |
 Whether to make the coins permanently visible. | | use_exit | True | Whether to
 spawn and use the exit task. The exit is accessible by the agent after
@@ -204,64 +218,62 @@
 global light. | | light_threshold | 255 | The threshold for dimming the global
 light. A value of 255 indicates that the light will dimmed of completely. | |
 visual_feedback | True | Whether to render the tiled background red if the
 agent is spotted. | | black_background | False | Whether to render the
 environments background black, while the spotlights are rendered as white
 circumferences. | | hide_chessboard | False | Whether to hide the chessboard
 background. This renders the background of the environment white. | |
+show_last_action | True | Whether to encode and render the previouss action to
+the visual observation. | | show_last_positive_reward | True | Whether to
+render if the agent received a positive reward on the previous step. | |
 reward_inside_spotlight | 0.0 | What reward to signal for each step while being
 inside a spotlight. | | reward_outside_spotlight | 0.0 | What reward to signal
 for each step while being outside of a spotlight. | | reward_death | 0.0 | What
 reward to signal upon losing all health points. | | reward_coin | 0.25 | What
 reward to signal upon collecting one coin. | ## Endless Searing Spotlights
 Endless Searing Spotlights solely revolves around a coin collection task, with
 no consideration of an exit task leading to episode termination. Upon
 collecting the only coin present, a new one is immediately spawned. The agent
 operates under a limited time budget to collect the newly spawned coin. ###
 Reset Parameters | Parameter | Default | Explanation | |-----------------------
 ---|--------:|-----------------------------------------------------------------
 ------------------------------------------------| | max_steps | -1 | The
 maximum number of steps for the agent to play one episode. | | agent_scale |
 0.25 | The dimensions of the agent. | | agent_speed | 3.0 | The speed of the
-agent. | | agent_health | 100 | The initial health points of the agent. | |
+agent. | | agent_health | 10 | The initial health points of the agent. | |
 agent_visible | False | Whether to make the agent permanently visible. | |
 sample_agent_position | True | Whether to hide or show the goal tile of the
-generated path. | | num_coins | [1] | The number of coins that are spawned.
-This is a list that the environment samples from. | | coin_scale | 0.375 | The
-scale of the coins. | | coins_visible | False | Whether to make the coins
-permanently visible. | | use_exit | True | Whether to spawn and use the exit
-task. The exit is accessible by the agent after collecting all coins. | |
-exit_scale | 0.0 | The scale of the exit. | | exit_visible | False | Whether to
-make the exit permanently visible. | | initial_spawns | 4 | The number of
-spotlights that are initially spawned. | | num_spawns | 30 | The number of
-spotlights that are to be spawned. | | initial_spawn_interval | 30 | The number
-of steps until the next spotlight is spawned. | | spawn_interval_threshold | 10
-| The spawn interval is decayed until reaching this lower threshold. | |
-spawn_interval_decay | 0.95 | The decay rate of the spotlight spawn interval. |
-| spot_min_radius | 7.5 | The minimum radius of the spotlights. The radius is
-sampled from the range min to max. | | spot_max_radius | 13.75 | The maximum
-radius of the spotlights. The radius is sampled from the range min to max. | |
-spot_min_speed | 0.0025 | The minimum speed of the spotlights. The speed is
-sampled from the range min to max. | | spot_max_speed | 0.0075 | The maximum
-speed of the spotlights. The speed is sampled from the range min to max. | |
-spot_damage | 1.0 | Damage per step while the agent is spotted by one
+generated path. | | coin_show_duration | 6 | How many steps to make the coin
+visible to the agent unill its hidden behind the dark. | | coin_scale | 0.375 |
+The scale of the coins. | | coins_visible | False | Whether to make the coins
+permanently visible. | | steps_per_coin | 160 | Time budget to collect a single
+coin. | | initial_spawns | 3 | The number of spotlights that are initially
+spawned. | | spawn_interval | 50 | The number of steps until the next spotlight
+is spawned. | | spot_min_radius | 7.5 | The minimum radius of the spotlights.
+The radius is sampled from the range min to max. | | spot_max_radius | 13.75 |
+The maximum radius of the spotlights. The radius is sampled from the range min
+to max. | | spot_min_speed | 0.0025 | The minimum speed of the spotlights. The
+speed is sampled from the range min to max. | | spot_max_speed | 0.0075 | The
+maximum speed of the spotlights. The speed is sampled from the range min to
+max. | | spot_damage | 1.0 | Damage per step while the agent is spotted by one
 spotlight. | | light_dim_off_duration | 6 | The number of steps to dim off the
 global light. | | light_threshold | 255 | The threshold for dimming the global
 light. A value of 255 indicates that the light will dimmed of completely. | |
 visual_feedback | True | Whether to render the tiled background red if the
 agent is spotted. | | black_background | False | Whether to render the
 environments background black, while the spotlights are rendered as white
 circumferences. | | hide_chessboard | False | Whether to hide the chessboard
 background. This renders the background of the environment white. | |
+show_last_action | True | Whether to encode and render the previouss action to
+the visual observation. | | show_last_positive_reward | True | Whether to
+render if the agent received a positive reward on the previous step. | |
 reward_inside_spotlight | 0.0 | What reward to signal for each step while being
 inside a spotlight. | | reward_outside_spotlight | 0.0 | What reward to signal
 for each step while being outside of a spotlight. | | reward_death | 0.0 | What
-reward to signal upon losing all health points. | | reward_exit | 1.0 | What
-reward to signal after successfully using the exit. | | reward_max_steps | 0.0
-| What reward to signal if max steps is reached. | | reward_coin | 0.25 | What
+reward to signal upon losing all health points. | | reward_coin | 0.25 | What
 reward to signal upon collecting one coin. | ## Training Baseline results are
 avaible via these repositories. [Recurrence + PPO](https://github.com/
 MarcoMeter/recurrent-ppo-truncated-bptt) [TransformerXL + PPO](https://
 github.com/MarcoMeter/episodic-transformer-memory-ppo) ## Changelog v1.0.0
 Improvements - All environment concepts are extrapolated to endless episodes! -
 Endless Mortar Mayhem - Endless Mystery Path - Endless Searing Spotlights -
 Improved simulation speed by using already rotated sprites and not rotating the
```

### Comparing `memory-gym-1.0.0/memory_gym/__init__.py` & `memory_gym-1.0.1/memory_gym/__init__.py`

 * *Files identical despite different names*

### Comparing `memory-gym-1.0.0/memory_gym/character_controller.py` & `memory_gym-1.0.1/memory_gym/character_controller.py`

 * *Files identical despite different names*

### Comparing `memory-gym-1.0.0/memory_gym/endless_mortar_mayhem.py` & `memory_gym-1.0.1/memory_gym/endless_mortar_mayhem.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,19 +75,19 @@
             pygame.event.set_allowed(None)
 
         # Init debug window
         self.debug_window = None      
 
         # Setup observation and action space
         self.action_space = spaces.MultiDiscrete([3, 3])
-        self.observation_space= spaces.Box(
-                    low = 0.0,
-                    high = 1.0,
+        self.observation_space= sspaces.Box(
+                    low = 0,
+                    high = 255,
                     shape = [self.screen_dim, self.screen_dim, 3],
-                    dtype = np.float32)
+                    dtype = np.uint8)
 
         # Optional information that is part of the returned info dictionary during reset and step
         # The absolute position (ground truth) of the agent is distributed using the info dictionary.
         self.has_ground_truth_info = True
         self.ground_truth_space = spaces.Box(
                     low = np.zeros((2), dtype=np.float32),
                     high = np.ones((2), dtype=np.float32),
@@ -249,15 +249,15 @@
         self._explosion_delay = self.np_random.choice(self.reset_params["explosion_delay"])
 
         # Draw
         self._draw_surfaces([(self.bg, (0, 0)), (self.arena.surface, self.arena.rect), self.agent.get_rotated_sprite(0),
                             (command.surface, (((self.screen_dim // 2) - command.rect_dim // 2, (self.screen_dim // 2) - command.rect_dim // 2)))])
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return vis_obs, {"ground_truth": np.asarray([*self._target_pos]) / 5.0} 
 
     def step(self, action):
         """Take a step in the environment.
 
         Arguments:
@@ -360,15 +360,15 @@
         # Draw
         surfaces = [(self.bg, (0, 0)), (self.arena.surface, self.arena.rect), (self.rotated_agent_surface, self.rotated_agent_rect)]
         if command is not None:
             surfaces.append((command.surface, ((self.screen_dim // 2) - command.rect_dim // 2, (self.screen_dim // 2) - command.rect_dim // 2)))
         self._draw_surfaces(surfaces)
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return vis_obs, reward, done, False, info
 
     def render(self):
         """Render the environment.
 
         Returns:
```

### Comparing `memory-gym-1.0.0/memory_gym/endless_mystery_path.py` & `memory_gym-1.0.1/memory_gym/endless_mystery_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,18 +77,18 @@
 
         # Init debug window
         self.debug_window = None
 
         # Setup observation and action space
         self.action_space = spaces.Discrete(4)
         self.observation_space= spaces.Box(
-                    low = 0.0,
-                    high = 1.0,
+                    low = 0,
+                    high = 255,
                     shape = [self.screen_dim, self.screen_dim, 3],
-                    dtype = np.float32)
+                    dtype = np.uint8)
         
         # Optional information that is part of the returned info dictionary during reset and step
         # The cardinal direction where the next path tile is located
         self.has_ground_truth_info = True
         self.ground_truth_space = spaces.Box(
                     low = np.zeros((3), dtype=np.float32),
                     high = np.ones((3), dtype=np.float32),
@@ -270,15 +270,15 @@
         # Draw
         if self.reset_params["show_stamina"]:
             self._draw_surfaces([(self.rotated_agent_surface, (self.agent_draw_x, self.rotated_agent_rect.y)), (self.stamina_surface, self.stamina_position)])
         else:
             self._draw_surfaces([(self.rotated_agent_surface, (self.agent_draw_x, self.rotated_agent_rect.y))])
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return vis_obs, {"ground_truth": self.target_direction}
 
     def step(self, action):
         """Take a step in the environment.
 
         Arguments:
@@ -432,15 +432,15 @@
         # Draw
         if self.reset_params["show_stamina"]:
             self._draw_surfaces([(self.rotated_agent_surface, (self.agent_draw_x, self.rotated_agent_rect.y)), (self.stamina_surface, self.stamina_position)])
         else:
             self._draw_surfaces([(self.rotated_agent_surface, (self.agent_draw_x, self.rotated_agent_rect.y))])
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return vis_obs, reward, done, False, info
 
     def render(self):
         """Render the environment.
 
         Returns:
```

### Comparing `memory-gym-1.0.0/memory_gym/endless_searing_spotlights.py` & `memory_gym-1.0.1/memory_gym/endless_searing_spotlights.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,18 +97,18 @@
 
         # Init debug window
         self.debug_window = None
 
         # Setup observation and action space
         self.action_space = spaces.MultiDiscrete([3, 3])
         self.observation_space= spaces.Box(
-                    low = 0.0,
-                    high = 1.0,
+                    low = 0,
+                    high = 255,
                     shape = [self.screen_dim, self.screen_dim, 3],
-                    dtype = np.float32)
+                    dtype = np.uint8)
         
         # Optional information that is part of the returned info dictionary during reset and step
         # The absolute position (ground truth) of the agent is distributed using the info dictionary.
         self.has_ground_truth_info = True
         self.ground_truth_space = spaces.Box(
                     low = np.zeros((4), dtype=np.float32),
                     high = np.ones((4), dtype=np.float32),
@@ -390,15 +390,15 @@
 
         # Show spawn mask for debugging purposes
         # import matplotlib.pyplot as plt
         # plt.imshow(np.flip(np.rot90(self.grid_sampler.spawn_mask), axis=0))
         # plt.show()
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         # Return the visual observation and the ground truth
         return vis_obs, {"ground_truth": np.concatenate((np.asarray(self.agent.rect.center), np.asarray(self.coin.location))) / self.screen_dim}
 
     def step(self, action):
         """Take a step in the environment.
 
@@ -484,15 +484,15 @@
                 # "mean_steps_between_coins": sum(self.steps_between_coins) / self.coins_collected
             }
         else:
             # Ground truth: agent and coin position
             info = {"ground_truth": np.concatenate((np.asarray(self.agent.rect.center), np.asarray(self.coin.location))) / self.screen_dim}
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return vis_obs, reward, done, False, info
 
     def close(self):
         """Close the environment."""
         if self.debug_window is not None:
             self.debug_window.destroy()
```

### Comparing `memory-gym-1.0.0/memory_gym/mortar_mayhem.py` & `memory_gym-1.0.1/memory_gym/mortar_mayhem.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,18 +78,18 @@
 
         # Init debug window
         self.debug_window = None      
 
         # Setup observation and action space
         self.action_space = spaces.MultiDiscrete([3, 3])
         self.observation_space= spaces.Box(
-                    low = 0.0,
-                    high = 1.0,
+                    low = 0,
+                    high = 255,
                     shape = [self.screen_dim, self.screen_dim, 3],
-                    dtype = np.float32)
+                    dtype = np.uint8)
 
         # Environment members
         self.rotated_agent_surface, self.rotated_agent_rect = None, None
 
     def _draw_surfaces(self, surfaces):
         """Draw all surfaces onto the Pygame screen.
 
@@ -263,15 +263,15 @@
         self._explosion_delay = self.np_random.choice(self.reset_params["explosion_delay"])
 
         # Draw
         self._draw_surfaces([(self.bg, (0, 0)), (self.arena.surface, self.arena.rect), self.agent.get_rotated_sprite(0),
                             (command.surface, (((self.screen_dim // 2) - command.rect_dim // 2, (self.screen_dim // 2) - command.rect_dim // 2)))])
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return vis_obs, {}
 
     def step(self, action):
         """Take a step in the environment.
 
         Arguments:
@@ -360,15 +360,15 @@
         # Draw
         surfaces = [(self.bg, (0, 0)), (self.arena.surface, self.arena.rect), (self.rotated_agent_surface, self.rotated_agent_rect)]
         if command is not None:
             surfaces.append((command.surface, ((self.screen_dim // 2) - command.rect_dim // 2, (self.screen_dim // 2) - command.rect_dim // 2)))
         self._draw_surfaces(surfaces)
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return vis_obs, reward, done, False, info
 
     def render(self):
         """Render the environment.
 
         Returns:
```

### Comparing `memory-gym-1.0.0/memory_gym/mortar_mayhem_b.py` & `memory_gym-1.0.1/memory_gym/mortar_mayhem_b.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     }
 
     default_reset_parameters = {
                 "agent_scale": 1.0 * SCALE,
                 "agent_speed": 12.0 * SCALE,
                 "arena_size": 5,
                 "allowed_commands": 9,
-                "command_count": [5],
+                "command_count": [10],
                 "explosion_duration": [6],
                 "explosion_delay": [18],
                 "visual_feedback": True,
                 "reward_command_failure": 0.0,
                 "reward_command_success": 0.1,
                 "reward_episode_success": 0.0
             }
@@ -54,15 +54,15 @@
 
     def __init__(self, render_mode = None) -> None:
         """Initialize the MortarMayhemTaskB Environment.
 
         Arguments:
             render_mode {str} -- The render mode for the environment. Default is None. (default: {None})
         """
-        super().__init__()
+        super().__init__(render_mode)
 
         self.render_mode = render_mode
         if render_mode is None:
             os.putenv('SDL_VIDEODRIVER', 'fbcon')
             os.environ["SDL_VIDEODRIVER"] = "dummy"
         else:
             pygame.display.set_caption("Environment")
@@ -80,18 +80,18 @@
 
         # Setup observation and action space
         self.max_num_commands = 20
         self.action_space = spaces.MultiDiscrete([3, 3])
         self.observation_space = spaces.Dict(
             {
                 "visual_observation": spaces.Box(
-                    low = 0.0,
-                    high = 1.0,
+                    low = 0,
+                    high = 255,
                     shape = [self.screen_dim, self.screen_dim, 3],
-                    dtype = np.float32),
+                    dtype = np.uint8),
                 "vector_observation": spaces.Box(
                     low = np.zeros((self.max_num_commands * 9), dtype=np.float32),
                     high = np.ones((self.max_num_commands * 9), dtype=np.float32),
                     shape = (self.max_num_commands * 9, ),
                     dtype = np.float32)
             }
         )
@@ -185,15 +185,15 @@
         self._explosion_duration = self.np_random.choice(self.reset_params["explosion_duration"])
         self._explosion_delay = self.np_random.choice(self.reset_params["explosion_delay"])
 
         # Draw
         self._draw_surfaces([(self.bg, (0, 0)), (self.arena.surface, self.arena.rect), self.agent.get_rotated_sprite(0)])
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
         # Retrieve the encoded commands for the observation space
         self._commands_one_hot = self._encode_commands_one_hot(self._commands)
 
         return {"visual_observation": vis_obs, "vector_observation": self._commands_one_hot}, {}
 
     def step(self, action):
         """Take a step in the environment.
@@ -279,15 +279,15 @@
         # Draw
         surfaces = [(self.bg, (0, 0)), (self.arena.surface, self.arena.rect), (self.rotated_agent_surface, self.rotated_agent_rect)]
         if command is not None:
             surfaces.append((command.surface, ((self.screen_dim // 2) - command.rect_dim // 2, (self.screen_dim // 2) - command.rect_dim // 2)))
         self._draw_surfaces(surfaces)
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return {"visual_observation": vis_obs, "vector_observation": self._commands_one_hot}, reward, done, False, info
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("--seed", type=int, help="The to be used seed for the environment's random number generator.", default=0)
     options = parser.parse_args()
```

### Comparing `memory-gym-1.0.0/memory_gym/mortar_mayhem_b_grid.py` & `memory_gym-1.0.1/memory_gym/mortar_mayhem_b_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     def __init__(self, render_mode = None) -> None:
         """Initialize the GridMortarMayhemTaskB Environment.
 
         Arguments:
             render_mode {str} -- The render mode for the environment. Default is None. (default: {None})
         """
-        super().__init__()
+        super().__init__(render_mode)
 
         self.render_mode = render_mode
         if render_mode is None:
             os.putenv('SDL_VIDEODRIVER', 'fbcon')
             os.environ["SDL_VIDEODRIVER"] = "dummy"
         else:
             pygame.display.set_caption("Environment")
@@ -79,18 +79,18 @@
 
         # Setup observation and action space
         self.max_num_commands = 20
         self.action_space = spaces.Discrete(4)
         self.observation_space = spaces.Dict(
             {
                 "visual_observation": spaces.Box(
-                    low = 0.0,
-                    high = 1.0,
+                    low = 0,
+                    high = 255,
                     shape = [self.screen_dim, self.screen_dim, 3],
-                    dtype = np.float32),
+                    dtype = np.uint8),
                 "vector_observation": spaces.Box(
                     low = np.zeros((self.max_num_commands * 9), dtype=np.float32),
                     high = np.ones((self.max_num_commands * 9), dtype=np.float32),
                     shape = (self.max_num_commands * 9, ),
                     dtype = np.float32)
             }
         )
@@ -183,15 +183,15 @@
         self._explosion_duration = self.np_random.choice(self.reset_params["explosion_duration"])
         self._explosion_delay = self.np_random.choice(self.reset_params["explosion_delay"])
 
         # Draw
         self._draw_surfaces([(self.bg, (0, 0)), (self.arena.surface, self.arena.rect), self.agent.get_rotated_sprite(0)])
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
         # Retrieve the encoded commands for the observation space
         self._commands_one_hot = self._encode_commands_one_hot(self._commands)
 
         return {"visual_observation": vis_obs, "vector_observation": self._commands_one_hot}, {}
 
     def step(self, action):
         """Take a step in the environment.
@@ -277,15 +277,15 @@
         # Draw
         surfaces = [(self.bg, (0, 0)), (self.arena.surface, self.arena.rect), (self.rotated_agent_surface, self.rotated_agent_rect)]
         if command is not None:
             surfaces.append((command.surface, ((self.screen_dim // 2) - command.rect_dim // 2, (self.screen_dim // 2) - command.rect_dim // 2)))
         self._draw_surfaces(surfaces)
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return {"visual_observation": vis_obs, "vector_observation": self._commands_one_hot}, reward, done, False, info
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("--seed", type=int, help="The to be used seed for the environment's random number generator.", default=0)
     options = parser.parse_args()
```

### Comparing `memory-gym-1.0.0/memory_gym/mortar_mayhem_grid.py` & `memory_gym-1.0.1/memory_gym/mortar_mayhem_grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,18 +77,18 @@
 
         # Init debug window
         self.debug_window = None      
 
         # Setup observation and action space
         self.action_space = spaces.Discrete(4)
         self.observation_space= spaces.Box(
-                    low = 0.0,
-                    high = 1.0,
+                    low = 0,
+                    high = 255,
                     shape = [self.screen_dim, self.screen_dim, 3],
-                    dtype = np.float32)
+                    dtype = np.uint8)
 
         # Environment members
         self.rotated_agent_surface, self.rotated_agent_rect = None, None
 
     def _draw_surfaces(self, surfaces):
         """Draw all surfaces onto the Pygame screen.
 
@@ -269,16 +269,16 @@
         self._explosion_delay = self.np_random.choice(self.reset_params["explosion_delay"])
 
         # Draw
         self._draw_surfaces([(self.bg, (0, 0)), (self.arena.surface, self.arena.rect), self.agent.get_rotated_sprite(0),
                             (command.surface, (((self.screen_dim // 2) - command.rect_dim // 2, (self.screen_dim // 2) - command.rect_dim // 2)))])
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
-
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        
         return vis_obs, {}
 
     def step(self, action):
         """Take a step in the environment.
 
         Arguments:
             action {list} -- The action to take.
@@ -366,15 +366,15 @@
         # Draw
         surfaces = [(self.bg, (0, 0)), (self.arena.surface, self.arena.rect), (self.rotated_agent_surface, self.rotated_agent_rect)]
         if command is not None:
             surfaces.append((command.surface, ((self.screen_dim // 2) - command.rect_dim // 2, (self.screen_dim // 2) - command.rect_dim // 2)))
         self._draw_surfaces(surfaces)
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return vis_obs, reward, done, False, info
 
     def render(self):
         """Render the environment.
 
         Returns:
```

### Comparing `memory-gym-1.0.0/memory_gym/mystery_path.py` & `memory_gym-1.0.1/memory_gym/mystery_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,18 +74,18 @@
 
         # Init debug window
         self.debug_window = None
 
         # Setup observation and action space
         self.action_space = spaces.MultiDiscrete([3, 3])
         self.observation_space= spaces.Box(
-                    low = 0.0,
-                    high = 1.0,
+                    low = 0,
+                    high = 255,
                     shape = [self.screen_dim, self.screen_dim, 3],
-                    dtype = np.float32)
+                    dtype = np.uint8)
         
         # Environment members
         self.rotated_agent_surface, self.rotated_agent_rect = None, None
         self.grid_dim = 7
         self.tile_dim = self.screen_dim / self.grid_dim
 
     def _draw_surfaces(self, surfaces):
@@ -191,15 +191,15 @@
         self.is_off_path = False
         self.num_fails = 0
 
         # Draw
         self._draw_surfaces([(self.path_surface, (0, 0)), (self.rotated_agent_surface, self.rotated_agent_rect)])
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return vis_obs, {}
 
     def step(self, action):
         """Take a step in the environment.
 
         Arguments:
@@ -267,15 +267,15 @@
         else:
             info = {}
 
         # Draw
         self._draw_surfaces([(self.path_surface, (0, 0)), (self.rotated_agent_surface, self.rotated_agent_rect), (self.fall_off_surface, self.fall_off_rect)])
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return vis_obs, reward, done, False, info
 
     def render(self):
         """Render the environment.
 
         Returns:
```

### Comparing `memory-gym-1.0.0/memory_gym/mystery_path_grid.py` & `memory_gym-1.0.1/memory_gym/mystery_path_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,18 +73,18 @@
 
         # Init debug window
         self.debug_window = None
 
         # Setup observation and action space
         self.action_space = spaces.Discrete(4)
         self.observation_space= spaces.Box(
-                    low = 0.0,
-                    high = 1.0,
+                    low = 0,
+                    high = 255,
                     shape = [self.screen_dim, self.screen_dim, 3],
-                    dtype = np.float32)
+                    dtype = np.uint8)
         
         # Environment members
         self.rotated_agent_surface, self.rotated_agent_rect = None, None
         self.grid_dim = 7
         self.tile_dim = self.screen_dim / self.grid_dim
 
     def _draw_surfaces(self, surfaces):
@@ -190,15 +190,15 @@
         self.is_off_path = False
         self.num_fails = 0
 
         # Draw
         self._draw_surfaces([(self.path_surface, (0, 0)), (self.rotated_agent_surface, self.rotated_agent_rect)])
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return vis_obs, {}
 
     def step(self, action):
         """Take a step in the environment.
 
         Arguments:
@@ -268,15 +268,15 @@
         else:
             info = {}
 
         # Draw
         self._draw_surfaces([(self.path_surface, (0, 0)), (self.rotated_agent_surface, self.rotated_agent_rect), (self.fall_off_surface, self.fall_off_rect)])
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return vis_obs, reward, done, False, info
 
     def render(self):
         """Render the environment.
 
         Returns:
```

### Comparing `memory-gym-1.0.0/memory_gym/pygame_assets.py` & `memory_gym-1.0.1/memory_gym/pygame_assets.py`

 * *Files identical despite different names*

### Comparing `memory-gym-1.0.0/memory_gym/searing_spotlights.py` & `memory_gym-1.0.1/memory_gym/searing_spotlights.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,28 +106,28 @@
 
         # Init debug window
         self.debug_window = None
 
         # Setup observation and action space
         self.action_space = spaces.MultiDiscrete([3, 3])
         self.observation_space= spaces.Box(
-                    low = 0.0,
-                    high = 1.0,
+                    low = 0,
+                    high = 255,
                     shape = [self.screen_dim, self.screen_dim, 3],
-                    dtype = np.float32)
+                    dtype = np.uint8)
 
         # Environment members
         # Tiled background surface
         self.blue_background_surface = get_tiled_background_surface(self.screen, self.screen_dim, (0, 0, 255), SCALE)
         self.red_background_surface = get_tiled_background_surface(self.screen, self.screen_dim, (255, 0, 0), SCALE)
 
         # Spotlight surface
         self.spotlight_surface = pygame.Surface((self.screen_dim, self.screen_dim))
         self.spotlight_surface.fill(0)
-        self.spotlight_surface.set_colorkey((255, 0, 0))
+        self.spotlight_surface.set_colorkey((255, 0, 0, 0))
 
         # Agent boundaries
         self.walkable_rect = pygame.Rect(0, 16 * SCALE, self.screen_dim, self.screen_dim - 16 * SCALE)
 
         # Init grid spawner
         self.grid_sampler = GridPositionSampler(self.screen_dim)
         # self.grid_sampler = GridPositionSampler(self.screen_dim - 16 * SCALE, self.screen_dim // 24)
@@ -440,15 +440,15 @@
 
         # Show spawn mask for debugging purposes
         # import matplotlib.pyplot as plt
         # plt.imshow(np.flip(np.rot90(self.grid_sampler.spawn_mask), axis=0))
         # plt.show()
 
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         # Return the visual observation and the ground truth
         return vis_obs, {}
 
     def step(self, action):
         """Take a step in the environment.
 
@@ -553,15 +553,15 @@
                 "coins_collected": self.coins_collected / self.num_coins,
                 "success": success
             }
         else:
             info = {}
         
         # Retrieve the rendered image of the environment
-        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.float32) / 255.0 # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        vis_obs = pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
 
         return vis_obs, reward, done, False, info
 
     def close(self):
         """Close the environment."""
         if self.debug_window is not None:
             self.debug_window.destroy()
```

### Comparing `memory-gym-1.0.0/memory_gym.egg-info/PKG-INFO` & `memory_gym-1.0.1/memory_gym.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: memory-gym
-Version: 1.0.0
+Version: 1.0.1
 Summary: A gym that contains the memory benchmarks Mortar Mayhem, Mystery Maze and Searing Spotlights
 Home-page: https://github.com/MarcoMeter/drl-memory-gym
 Author: Marco Pleines
 Project-URL: Github, https://github.com/MarcoMeter/drl-memory-gym
 Project-URL: Bug Tracker, https://github.com/MarcoMeter/drl-memory-gym/issues
 Keywords: Deep Reinforcement Learning,gym,POMDP,Imperfect Information,Partial Observation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: gymnasium==0.29.0
+Requires-Dist: pygame==2.4.0
 
-[[Paper](https://openreview.net/forum?id=jHc8dCx6DDr)] [[Installation](#installation)]  [[Usage](#usage)] [[Mortar Mayhem](#mortar-mayhem)] [[Endless Mortar Mayhem](#endless-mortar-mayhem)] [[Mystery Path](#mystery-path)] [[Endless Mystery Path](#enndless-mystery-path)] [[Searing Spotlights](#searing-spotlights)] [[Endless Searing Spotlights](#endless-searing-spotlights)] [[Training](#training)]
+[[Paper](https://arxiv.org/abs/2309.17207)] [[Installation](#installation)]  [[Usage](#usage)] [[Mortar Mayhem](#mortar-mayhem)] [[Endless Mortar Mayhem](#endless-mortar-mayhem)] [[Mystery Path](#mystery-path)] [[Endless Mystery Path](#endless-mystery-path)] [[Searing Spotlights](#searing-spotlights)] [[Endless Searing Spotlights](#endless-searing-spotlights)] [[Training](#training)]
 
-# Memory Gym: Partially Observable Challenges to Memory-Based Agents in Endless Episodes
+# Memory Gym: Towards Endless Tasks to Benchmark Memory Capabilities of Agents
 
 <table align="center">
   <tr>
     <td></td>
     <td>Endless Mortar Mayhem</td>
     <td>Endless Mystery Path</td>
     <td>Endless Searing Spotlights</td>
@@ -36,30 +38,40 @@
     <td><img src="docs/assets/emm_0_gt.gif" width=180></td>
     <td><img src="docs/assets/emp_0_gt.gif" width=180></td>
     <td><img src="docs/assets/ess_0_gt.gif" width=180></td>
   </tr>
 </table>
 
 
-Memory Gym features the environments **Mortar Mayhem**, **Mystery Path**, and **Searing Spotlights** that are inspired by some mini games of [Pummel Party](http://rebuiltgames.com/). These environments shall benchmark an agent's memory to
-- memorize events across long sequences,
-- generalize,
-- and be robust to noise.
-
-Especially, these environments feature endless task variants. As the agent's policy improves, the task goes on. The traveling game "I packed my bag ..." inspired this dynamic concept, which allows for examining levels of effectinvess instead of just sample efficiency.
+Memory Gym features the environments **Mortar Mayhem**, **Mystery Path**, and **Searing Spotlights** that are inspired by some mini games of [Pummel Party](http://rebuiltgames.com/). These 2D environments benchmark the memory capabilities of agents.
+Especially, these environments feature endless task variants. As the agent's policy improves, the task goes on. The cumulative memory game "I packed my bag ..." inspired this dynamic concept, which allows for examining levels of effectiveness instead of just sample efficiency.
+Interactive videos, based on selected agent behavios, can be found here: https://marcometer.github.io/
 
 ## Citation
 
+Preprint Journal Paper (under review)
+```bibtex
+@misc{pleines2024memory,
+      title={Memory Gym: Towards Endless Tasks to Benchmark Memory Capabilities of Agents}, 
+      author={Marco Pleines and Matthias Pallasch and Frank Zimmer and Mike Preuss},
+      year={2024},
+      eprint={2309.17207},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG}
+}
+```
+
+ICLR Paper
 ```bibtex
 @inproceedings{pleines2023memory,
-title={Memory Gym: Partially Observable Challenges to Memory-Based Agents},
-author={Marco Pleines and Matthias Pallasch and Frank Zimmer and Mike Preuss},
-booktitle={International Conference on Learning Representations},
-year={2023},
-url={https://openreview.net/forum?id=jHc8dCx6DDr}
+      title={Memory Gym: Partially Observable Challenges to Memory-Based Agents},
+      author={Marco Pleines and Matthias Pallasch and Frank Zimmer and Mike Preuss},
+      booktitle={International Conference on Learning Representations},
+      year={2023},
+      url={https://openreview.net/forum?id=jHc8dCx6DDr}
 }
 ```
 
 ## Installation
 
 Major dependencies:
 - gymnasium==0.29.0
@@ -282,15 +294,15 @@
 
 | Parameter                | Default | Explanation                                                                                                     |
 |--------------------------|--------:|-----------------------------------------------------------------------------------------------------------------|
 | max_steps                |     -1 | The maximum number of steps for the agent to play one episode. If smaller than 1, the episode is not affected by this reset parameter.                                                  |
 | steps_per_coin                |     160 | Number of steps that the agent has to collect a newly spawned coin.                                                  |
 | agent_scale              |    0.25 | The dimensions of the agent.                                                                                    |
 | agent_speed              |     3.0 | The speed of the agent.                                                                                         |
-| agent_health             |     10 | The initial health points of the agent.                                                                         |
+| agent_health             |     5 | The initial health points of the agent.                                                                         |
 | agent_visible            |   False | Whether to make the agent permanently visible.                                                                  |
 | sample_agent_position    |    True | Whether to hide or show the goal tile of the generated path.                                                    |
 | num_coins                |     [1] | The number of coins that are spawned. This is a list that the environment samples from.                         |
 | coin_scale               |   0.375 | The scale of the coins.                                                                                         |
 | coins_visible            |   False | Whether to make the coins permanently visible.                                                                  |
 | use_exit                 |    True | Whether to spawn and use the exit task. The exit is accessible by the agent after collecting all coins.         |
 | exit_scale               |     0.0 | The scale of the exit.                                                                                          |
@@ -303,14 +315,16 @@
 | spot_max_speed           | 0.0075  | The maximum speed of the spotlights. The speed is sampled from the range min to max.                            |
 | spot_damage              | 1.0     | Damage per step while the agent is spotted by one spotlight.                                                    |
 | light_dim_off_duration   | 6       | The number of steps to dim off the global light.                                                                |
 | light_threshold          | 255     | The threshold for dimming the global light. A value of 255 indicates that the light will dimmed of completely.  |
 | visual_feedback          | True    | Whether to render the tiled background red if the agent is spotted.                                             |
 | black_background         | False   | Whether to render the environments background black, while the spotlights are rendered as white circumferences. |
 | hide_chessboard          | False   | Whether to hide the chessboard background. This renders the background of the environment white.                           |
+| show_last_action         | True    | Whether to encode and render the previouss action to the visual observation.                                    |
+| show_last_positive_reward | True   | Whether to render if the agent received a positive reward on the previous step.                                 |
 | reward_inside_spotlight  | 0.0     | What reward to signal for each step while being inside a spotlight.                                             |
 | reward_outside_spotlight | 0.0     | What reward to signal for each step while being outside of a spotlight.                                         |
 | reward_death             | 0.0     | What reward to signal upon losing all health points.                                                            |
 | reward_coin              | 0.25    | What reward to signal upon collecting one coin.                                                                 |
 
 ## Endless Searing Spotlights
 
@@ -319,43 +333,38 @@
 ### Reset Parameters
 
 | Parameter                | Default | Explanation                                                                                                     |
 |--------------------------|--------:|-----------------------------------------------------------------------------------------------------------------|
 | max_steps                |     -1 | The maximum number of steps for the agent to play one episode.                                                  |
 | agent_scale              |    0.25 | The dimensions of the agent.                                                                                    |
 | agent_speed              |     3.0 | The speed of the agent.                                                                                         |
-| agent_health             |     100 | The initial health points of the agent.                                                                         |
+| agent_health             |     10 | The initial health points of the agent.                                                                         |
 | agent_visible            |   False | Whether to make the agent permanently visible.                                                                  |
 | sample_agent_position    |    True | Whether to hide or show the goal tile of the generated path.                                                    |
-| num_coins                |     [1] | The number of coins that are spawned. This is a list that the environment samples from.                         |
+| coin_show_duration       |     6 | How many steps to make the coin visible to the agent unill its hidden behind the dark.                         |
 | coin_scale               |   0.375 | The scale of the coins.                                                                                         |
 | coins_visible            |   False | Whether to make the coins permanently visible.                                                                  |
-| use_exit                 |    True | Whether to spawn and use the exit task. The exit is accessible by the agent after collecting all coins.         |
-| exit_scale               |     0.0 | The scale of the exit.                                                                                          |
-| exit_visible             | False   | Whether to make the exit permanently visible.                                                                   |
-| initial_spawns           | 4       | The number of spotlights that are initially spawned.                                                            |
-| num_spawns               | 30      | The number of spotlights that are to be spawned.                                                                |
-| initial_spawn_interval   | 30      | The number of steps until the next spotlight is spawned.                                                        |
-| spawn_interval_threshold | 10      | The spawn interval is decayed until reaching this lower threshold.                                              |
-| spawn_interval_decay     | 0.95    | The decay rate of the spotlight spawn interval.                                                                 |
+| steps_per_coin            |   160 | Time budget to collect a single coin.                                                                  |
+| initial_spawns           | 3       | The number of spotlights that are initially spawned.                                                            |
+| spawn_interval   | 50      | The number of steps until the next spotlight is spawned.                                                        |
 | spot_min_radius          | 7.5     | The minimum radius of the spotlights. The radius is sampled from the range min to max.                          |
 | spot_max_radius          | 13.75   | The maximum radius of the spotlights. The radius is sampled from the range min to max.                          |
 | spot_min_speed           | 0.0025  | The minimum speed of the spotlights. The speed is sampled from the range min to max.                            |
 | spot_max_speed           | 0.0075  | The maximum speed of the spotlights. The speed is sampled from the range min to max.                            |
 | spot_damage              | 1.0     | Damage per step while the agent is spotted by one spotlight.                                                    |
 | light_dim_off_duration   | 6       | The number of steps to dim off the global light.                                                                |
 | light_threshold          | 255     | The threshold for dimming the global light. A value of 255 indicates that the light will dimmed of completely.  |
 | visual_feedback          | True    | Whether to render the tiled background red if the agent is spotted.                                             |
 | black_background         | False   | Whether to render the environments background black, while the spotlights are rendered as white circumferences. |
 | hide_chessboard          | False   | Whether to hide the chessboard background. This renders the background of the environment white.                           |
+| show_last_action         | True    | Whether to encode and render the previouss action to the visual observation.                                    |
+| show_last_positive_reward | True   | Whether to render if the agent received a positive reward on the previous step.                                 |
 | reward_inside_spotlight  | 0.0     | What reward to signal for each step while being inside a spotlight.                                             |
 | reward_outside_spotlight | 0.0     | What reward to signal for each step while being outside of a spotlight.                                         |
 | reward_death             | 0.0     | What reward to signal upon losing all health points.                                                            |
-| reward_exit              | 1.0     | What reward to signal after successfully using the exit.                                                        |
-| reward_max_steps         | 0.0     | What reward to signal if max steps is reached.                                                                  |
 | reward_coin              | 0.25    | What reward to signal upon collecting one coin.                                                                 |
 
 ## Training
 
 Baseline results are avaible via these repositories.
 
 [Recurrence + PPO](https://github.com/MarcoMeter/recurrent-ppo-truncated-bptt)
```

#### html2text {}

```diff
@@ -1,37 +1,42 @@
-Metadata-Version: 2.1 Name: memory-gym Version: 1.0.0 Summary: A gym that
+Metadata-Version: 2.1 Name: memory-gym Version: 1.0.1 Summary: A gym that
 contains the memory benchmarks Mortar Mayhem, Mystery Maze and Searing
 Spotlights Home-page: https://github.com/MarcoMeter/drl-memory-gym Author:
 Marco Pleines Project-URL: Github, https://github.com/MarcoMeter/drl-memory-gym
 Project-URL: Bug Tracker, https://github.com/MarcoMeter/drl-memory-gym/issues
 Keywords: Deep Reinforcement Learning,gym,POMDP,Imperfect Information,Partial
 Observation Classifier: Programming Language :: Python :: 3 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE [[Paper](https://openreview.net/forum?id=jHc8dCx6DDr)] [[Installation]
-(#installation)] [[Usage](#usage)] [[Mortar Mayhem](#mortar-mayhem)] [[Endless
-Mortar Mayhem](#endless-mortar-mayhem)] [[Mystery Path](#mystery-path)] [
-[Endless Mystery Path](#enndless-mystery-path)] [[Searing Spotlights](#searing-
-spotlights)] [[Endless Searing Spotlights](#endless-searing-spotlights)] [
-[Training](#training)] # Memory Gym: Partially Observable Challenges to Memory-
-Based Agents in Endless Episodes
+LICENSE Requires-Dist: gymnasium==0.29.0 Requires-Dist: pygame==2.4.0 [[Paper]
+(https://arxiv.org/abs/2309.17207)] [[Installation](#installation)] [[Usage]
+(#usage)] [[Mortar Mayhem](#mortar-mayhem)] [[Endless Mortar Mayhem](#endless-
+mortar-mayhem)] [[Mystery Path](#mystery-path)] [[Endless Mystery Path]
+(#endless-mystery-path)] [[Searing Spotlights](#searing-spotlights)] [[Endless
+Searing Spotlights](#endless-searing-spotlights)] [[Training](#training)] #
+Memory Gym: Towards Endless Tasks to Benchmark Memory Capabilities of Agents
                    Endless Mortar Mayhem Endless Mystery Path Endless Searing
                                                               Spotlights
  Agent Observation [docs/assets/         [docs/assets/        [docs/assets/
                    emm_0.gif]            emp_0.gif]           ess_0.gif]
  Ground Truth      [docs/assets/         [docs/assets/        [docs/assets/
                    emm_0_gt.gif]         emp_0_gt.gif]        ess_0_gt.gif]
 Memory Gym features the environments **Mortar Mayhem**, **Mystery Path**, and
 **Searing Spotlights** that are inspired by some mini games of [Pummel Party]
-(http://rebuiltgames.com/). These environments shall benchmark an agent's
-memory to - memorize events across long sequences, - generalize, - and be
-robust to noise. Especially, these environments feature endless task variants.
-As the agent's policy improves, the task goes on. The traveling game "I packed
-my bag ..." inspired this dynamic concept, which allows for examining levels of
-effectinvess instead of just sample efficiency. ## Citation ```bibtex
+(http://rebuiltgames.com/). These 2D environments benchmark the memory
+capabilities of agents. Especially, these environments feature endless task
+variants. As the agent's policy improves, the task goes on. The cumulative
+memory game "I packed my bag ..." inspired this dynamic concept, which allows
+for examining levels of effectiveness instead of just sample efficiency.
+Interactive videos, based on selected agent behavios, can be found here: https:
+//marcometer.github.io/ ## Citation Preprint Journal Paper (under review)
+```bibtex @misc{pleines2024memory, title={Memory Gym: Towards Endless Tasks to
+Benchmark Memory Capabilities of Agents}, author={Marco Pleines and Matthias
+Pallasch and Frank Zimmer and Mike Preuss}, year={2024}, eprint={2309.17207},
+archivePrefix={arXiv}, primaryClass={cs.LG} } ``` ICLR Paper ```bibtex
 @inproceedings{pleines2023memory, title={Memory Gym: Partially Observable
 Challenges to Memory-Based Agents}, author={Marco Pleines and Matthias Pallasch
 and Frank Zimmer and Mike Preuss}, booktitle={International Conference on
 Learning Representations}, year={2023}, url={https://openreview.net/
 forum?id=jHc8dCx6DDr} } ``` ## Installation Major dependencies: -
 gymnasium==0.29.0 - PyGame==2.4.0 ```console conda create -n memory-gym
 python=3.11 --yes conda activate memory-gym pip install memory-gym ``` or
@@ -186,15 +191,15 @@
 docs/assets/spots.jpg) ### Reset Parameters | Parameter | Default | Explanation
 | |--------------------------|--------:|---------------------------------------
 --------------------------------------------------------------------------| |
 max_steps | -1 | The maximum number of steps for the agent to play one episode.
 If smaller than 1, the episode is not affected by this reset parameter. | |
 steps_per_coin | 160 | Number of steps that the agent has to collect a newly
 spawned coin. | | agent_scale | 0.25 | The dimensions of the agent. | |
-agent_speed | 3.0 | The speed of the agent. | | agent_health | 10 | The initial
+agent_speed | 3.0 | The speed of the agent. | | agent_health | 5 | The initial
 health points of the agent. | | agent_visible | False | Whether to make the
 agent permanently visible. | | sample_agent_position | True | Whether to hide
 or show the goal tile of the generated path. | | num_coins | [1] | The number
 of coins that are spawned. This is a list that the environment samples from. |
 | coin_scale | 0.375 | The scale of the coins. | | coins_visible | False |
 Whether to make the coins permanently visible. | | use_exit | True | Whether to
 spawn and use the exit task. The exit is accessible by the agent after
@@ -213,64 +218,62 @@
 global light. | | light_threshold | 255 | The threshold for dimming the global
 light. A value of 255 indicates that the light will dimmed of completely. | |
 visual_feedback | True | Whether to render the tiled background red if the
 agent is spotted. | | black_background | False | Whether to render the
 environments background black, while the spotlights are rendered as white
 circumferences. | | hide_chessboard | False | Whether to hide the chessboard
 background. This renders the background of the environment white. | |
+show_last_action | True | Whether to encode and render the previouss action to
+the visual observation. | | show_last_positive_reward | True | Whether to
+render if the agent received a positive reward on the previous step. | |
 reward_inside_spotlight | 0.0 | What reward to signal for each step while being
 inside a spotlight. | | reward_outside_spotlight | 0.0 | What reward to signal
 for each step while being outside of a spotlight. | | reward_death | 0.0 | What
 reward to signal upon losing all health points. | | reward_coin | 0.25 | What
 reward to signal upon collecting one coin. | ## Endless Searing Spotlights
 Endless Searing Spotlights solely revolves around a coin collection task, with
 no consideration of an exit task leading to episode termination. Upon
 collecting the only coin present, a new one is immediately spawned. The agent
 operates under a limited time budget to collect the newly spawned coin. ###
 Reset Parameters | Parameter | Default | Explanation | |-----------------------
 ---|--------:|-----------------------------------------------------------------
 ------------------------------------------------| | max_steps | -1 | The
 maximum number of steps for the agent to play one episode. | | agent_scale |
 0.25 | The dimensions of the agent. | | agent_speed | 3.0 | The speed of the
-agent. | | agent_health | 100 | The initial health points of the agent. | |
+agent. | | agent_health | 10 | The initial health points of the agent. | |
 agent_visible | False | Whether to make the agent permanently visible. | |
 sample_agent_position | True | Whether to hide or show the goal tile of the
-generated path. | | num_coins | [1] | The number of coins that are spawned.
-This is a list that the environment samples from. | | coin_scale | 0.375 | The
-scale of the coins. | | coins_visible | False | Whether to make the coins
-permanently visible. | | use_exit | True | Whether to spawn and use the exit
-task. The exit is accessible by the agent after collecting all coins. | |
-exit_scale | 0.0 | The scale of the exit. | | exit_visible | False | Whether to
-make the exit permanently visible. | | initial_spawns | 4 | The number of
-spotlights that are initially spawned. | | num_spawns | 30 | The number of
-spotlights that are to be spawned. | | initial_spawn_interval | 30 | The number
-of steps until the next spotlight is spawned. | | spawn_interval_threshold | 10
-| The spawn interval is decayed until reaching this lower threshold. | |
-spawn_interval_decay | 0.95 | The decay rate of the spotlight spawn interval. |
-| spot_min_radius | 7.5 | The minimum radius of the spotlights. The radius is
-sampled from the range min to max. | | spot_max_radius | 13.75 | The maximum
-radius of the spotlights. The radius is sampled from the range min to max. | |
-spot_min_speed | 0.0025 | The minimum speed of the spotlights. The speed is
-sampled from the range min to max. | | spot_max_speed | 0.0075 | The maximum
-speed of the spotlights. The speed is sampled from the range min to max. | |
-spot_damage | 1.0 | Damage per step while the agent is spotted by one
+generated path. | | coin_show_duration | 6 | How many steps to make the coin
+visible to the agent unill its hidden behind the dark. | | coin_scale | 0.375 |
+The scale of the coins. | | coins_visible | False | Whether to make the coins
+permanently visible. | | steps_per_coin | 160 | Time budget to collect a single
+coin. | | initial_spawns | 3 | The number of spotlights that are initially
+spawned. | | spawn_interval | 50 | The number of steps until the next spotlight
+is spawned. | | spot_min_radius | 7.5 | The minimum radius of the spotlights.
+The radius is sampled from the range min to max. | | spot_max_radius | 13.75 |
+The maximum radius of the spotlights. The radius is sampled from the range min
+to max. | | spot_min_speed | 0.0025 | The minimum speed of the spotlights. The
+speed is sampled from the range min to max. | | spot_max_speed | 0.0075 | The
+maximum speed of the spotlights. The speed is sampled from the range min to
+max. | | spot_damage | 1.0 | Damage per step while the agent is spotted by one
 spotlight. | | light_dim_off_duration | 6 | The number of steps to dim off the
 global light. | | light_threshold | 255 | The threshold for dimming the global
 light. A value of 255 indicates that the light will dimmed of completely. | |
 visual_feedback | True | Whether to render the tiled background red if the
 agent is spotted. | | black_background | False | Whether to render the
 environments background black, while the spotlights are rendered as white
 circumferences. | | hide_chessboard | False | Whether to hide the chessboard
 background. This renders the background of the environment white. | |
+show_last_action | True | Whether to encode and render the previouss action to
+the visual observation. | | show_last_positive_reward | True | Whether to
+render if the agent received a positive reward on the previous step. | |
 reward_inside_spotlight | 0.0 | What reward to signal for each step while being
 inside a spotlight. | | reward_outside_spotlight | 0.0 | What reward to signal
 for each step while being outside of a spotlight. | | reward_death | 0.0 | What
-reward to signal upon losing all health points. | | reward_exit | 1.0 | What
-reward to signal after successfully using the exit. | | reward_max_steps | 0.0
-| What reward to signal if max steps is reached. | | reward_coin | 0.25 | What
+reward to signal upon losing all health points. | | reward_coin | 0.25 | What
 reward to signal upon collecting one coin. | ## Training Baseline results are
 avaible via these repositories. [Recurrence + PPO](https://github.com/
 MarcoMeter/recurrent-ppo-truncated-bptt) [TransformerXL + PPO](https://
 github.com/MarcoMeter/episodic-transformer-memory-ppo) ## Changelog v1.0.0
 Improvements - All environment concepts are extrapolated to endless episodes! -
 Endless Mortar Mayhem - Endless Mystery Path - Endless Searing Spotlights -
 Improved simulation speed by using already rotated sprites and not rotating the
```

### Comparing `memory-gym-1.0.0/memory_gym.egg-info/SOURCES.txt` & `memory_gym-1.0.1/memory_gym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `memory-gym-1.0.0/memory_gym.egg-info/entry_points.txt` & `memory_gym-1.0.1/memory_gym.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `memory-gym-1.0.0/setup.py` & `memory_gym-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,9 +45,9 @@
             "mortar_mayhem_grid=memory_gym.mortar_mayhem_grid:main",
             "mortar_mayhem_b_grid=memory_gym.mortar_mayhem_b_grid:main",
             "mystery_path=memory_gym.mystery_path:main",
             "endless_mystery_path=memory_gym.endless_mystery_path:main",
             "mystery_path_grid=memory_gym.mystery_path_grid:main",
             ],
       },
-      version="1.0.0",
+      version="1.0.1",
 )
```

