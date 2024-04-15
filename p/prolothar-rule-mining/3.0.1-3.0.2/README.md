# Comparing `tmp/prolothar-rule-mining-3.0.1.tar.gz` & `tmp/prolothar-rule-mining-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prolothar-rule-mining-3.0.1.tar", last modified: Fri Feb 16 11:54:44 2024, max compression
+gzip compressed data, was "prolothar-rule-mining-3.0.2.tar", last modified: Sat Apr 13 07:34:32 2024, max compression
```

## Comparing `prolothar-rule-mining-3.0.1.tar` & `prolothar-rule-mining-3.0.2.tar`

### file list

```diff
@@ -1,175 +1,180 @@
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.215807 prolothar-rule-mining-3.0.1/
--rw-rw-rw-   0        0        0    35821 2024-02-14 09:05:22.000000 prolothar-rule-mining-3.0.1/LICENSE
--rw-rw-rw-   0        0        0      538 2024-02-16 11:53:11.000000 prolothar-rule-mining-3.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4057 2024-02-16 11:54:44.213820 prolothar-rule-mining-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3342 2024-02-16 10:16:10.000000 prolothar-rule-mining-3.0.1/README.md
--rw-rw-rw-   0        0        0   105071 2024-02-15 13:38:27.000000 prolothar-rule-mining-3.0.1/coverage.xml
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:43.897114 prolothar-rule-mining-3.0.1/prolothar_rule_mining/
--rw-rw-rw-   0        0        0      811 2024-02-15 13:30:07.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:43.956883 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/
--rw-rw-rw-   0        0        0        0 2021-06-25 09:04:07.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/__init__.py
--rw-rw-rw-   0        0        0  2311866 2024-02-15 13:31:13.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/conditions.cpp
--rw-rw-rw-   0        0        0    22659 2024-02-15 13:12:21.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/conditions.pyx
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:43.963195 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/converter/
--rw-rw-rw-   0        0        0     3068 2024-02-15 13:12:21.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/converter/eventflow_graph_to_pm4py_petrinet_converter.py
--rw-rw-rw-   0        0        0     2603 2024-02-15 13:12:30.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/converter/sequence_to_class_dataset_converter.py
--rw-rw-rw-   0        0        0     2016 2024-02-15 13:12:33.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/converter/sequence_to_multilabel_dataset_converter.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:43.972672 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/dataset_generator/
--rw-rw-rw-   0        0        0     1120 2024-02-15 13:12:37.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/dataset_generator/__init__.py
--rw-rw-rw-   0        0        0     4529 2024-02-15 13:12:46.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/dataset_generator/classification.py
--rw-rw-rw-   0        0        0    17267 2024-02-15 13:12:49.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/dataset_generator/data_to_sequence.py
--rw-rw-rw-   0        0        0     5270 2024-02-15 13:12:21.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/dataset_generator/dataset_generator.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:43.986672 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/
--rw-rw-rw-   0        0        0     1089 2024-02-15 13:15:25.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.026673 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/
--rw-rw-rw-   0        0        0        0 2021-06-25 09:04:07.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/__init__.py
--rw-rw-rw-   0        0        0   341763 2024-02-15 13:31:13.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/a_star.cpp
--rw-rw-rw-   0        0        0     2151 2024-02-15 13:14:07.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/a_star.pyx
--rw-rw-rw-   0        0        0   671330 2024-02-15 13:31:13.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/alignment.cpp
--rw-rw-rw-   0        0        0     2594 2024-02-15 13:13:45.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/alignment.pyx
--rw-rw-rw-   0        0        0   382256 2024-02-15 13:31:13.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/alignment_finder.cpp
--rw-rw-rw-   0        0        0     1451 2024-02-15 13:13:32.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/alignment_finder.pyx
--rw-rw-rw-   0        0        0     2464 2024-02-15 13:13:50.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/beam_search.py
--rw-rw-rw-   0        0        0     2515 2024-02-15 13:13:55.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/greedy_beam_search.py
--rw-rw-rw-   0        0        0     3861 2024-02-15 13:14:00.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/greedy_shortest_path.py
--rw-rw-rw-   0        0        0   796662 2024-02-15 13:31:13.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/heuristics.cpp
--rw-rw-rw-   0        0        0     8191 2024-02-15 13:14:13.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/heuristics.pyx
--rw-rw-rw-   0        0        0   599233 2024-02-15 13:31:13.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/partial_alignment.cpp
--rw-rw-rw-   0        0        0     4847 2024-02-15 13:14:22.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/partial_alignment.pyx
--rw-rw-rw-   0        0        0  1327970 2024-02-15 13:31:14.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/path_enumeration.cpp
--rw-rw-rw-   0        0        0     5945 2024-02-15 13:14:28.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/path_enumeration.pyx
--rw-rw-rw-   0        0        0     3092 2024-02-15 13:14:32.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/petrinet.py
--rw-rw-rw-   0        0        0     3093 2024-02-15 13:14:36.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/sync_or_log_only.py
--rw-rw-rw-   0        0        0     2509 2024-02-15 13:15:29.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/caching.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.033685 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/cover/
--rw-rw-rw-   0        0        0     1458 2024-02-15 13:14:42.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/cover/__init__.py
--rw-rw-rw-   0        0        0     8167 2024-02-15 13:14:50.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/cover/cover.py
--rw-rw-rw-   0        0        0     4829 2024-02-15 13:14:47.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/cover/cover_computer.py
--rw-rw-rw-   0        0        0     2428 2024-02-15 13:14:53.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/cover/model_code_counter.py
--rw-rw-rw-   0        0        0     1613 2024-02-15 13:15:33.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/edge.py
--rw-rw-rw-   0        0        0    23288 2024-02-16 10:10:05.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/graph.py
--rw-rw-rw-   0        0        0   438183 2024-02-15 13:31:14.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/node.cpp
--rw-rw-rw-   0        0        0     2249 2024-02-15 13:15:44.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/node.pyx
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.038693 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/router/
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.044670 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/router/learning/
--rw-rw-rw-   0        0        0     1062 2024-02-15 13:15:00.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/router/learning/__init__.py
--rw-rw-rw-   0        0        0     2606 2024-02-15 13:15:03.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/router/learning/oracle_router_learner.py
--rw-rw-rw-   0        0        0     2841 2024-02-15 13:15:06.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/router/learning/rule_classifier_router_learner.py
--rw-rw-rw-   0        0        0     2723 2024-02-15 13:15:10.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/router/oracle_router.py
--rw-rw-rw-   0        0        0     1085 2024-02-15 13:15:14.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/router/router.py
--rw-rw-rw-   0        0        0     1707 2024-02-15 13:15:18.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/router/ruled_router.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.049672 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/
--rw-rw-rw-   0        0        0      811 2024-02-15 13:30:01.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.051699 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/
--rw-rw-rw-   0        0        0      811 2024-02-15 13:18:29.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.055699 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/knn/
--rw-rw-rw-   0        0        0      894 2024-02-15 13:16:22.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/knn/__init__.py
--rw-rw-rw-   0        0        0     2859 2024-02-16 08:41:33.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/knn/knn.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.061672 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/naive_bayes/
--rw-rw-rw-   0        0        0     1057 2024-02-15 13:16:38.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/naive_bayes/__init__.py
--rw-rw-rw-   0        0        0     3521 2024-02-15 13:12:21.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/naive_bayes/categorical_naive_bayes.py
--rw-rw-rw-   0        0        0     2885 2024-02-15 13:12:21.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/naive_bayes/mixed_naive_bayes.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.067674 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/
--rw-rw-rw-   0        0        0      914 2024-02-15 13:17:30.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/__init__.py
--rw-rw-rw-   0        0        0     2672 2024-02-15 13:17:40.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/candidate.py
--rw-rw-rw-   0        0        0     5265 2024-02-15 13:12:21.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/reliable_rule_miner.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.075694 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/strategy/
--rw-rw-rw-   0        0        0   894842 2024-02-15 13:31:14.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/strategy/abstract.cpp
--rw-rw-rw-   0        0        0    13305 2024-02-15 13:17:07.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/strategy/abstract.pyx
--rw-rw-rw-   0        0        0     6866 2024-02-15 13:17:10.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/strategy/beam_search.py
--rw-rw-rw-   0        0        0     4489 2024-02-15 13:17:21.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/strategy/best_first.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.093922 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/
--rw-rw-rw-   0        0        0     1396 2024-02-15 13:18:02.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/__init__.py
--rw-rw-rw-   0        0        0      962 2024-02-15 13:17:59.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/class_output_exception.py
--rw-rw-rw-   0        0        0     2436 2024-02-15 13:18:06.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/first_firing_rule_model.py
--rw-rw-rw-   0        0        0     4227 2024-02-15 13:18:10.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/if_then_else_rule.py
--rw-rw-rw-   0        0        0     3811 2024-02-15 13:18:13.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/list_of_rules.py
--rw-rw-rw-   0        0        0     2316 2024-02-15 13:18:17.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/return_class_rule.py
--rw-rw-rw-   0        0        0     1893 2024-02-15 13:18:20.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/rule.py
--rw-rw-rw-   0        0        0     5337 2024-02-16 09:30:36.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/sklearn.py
--rw-rw-rw-   0        0        0     1931 2024-02-15 13:18:27.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/voting_class_rule.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.099943 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/
--rw-rw-rw-   0        0        0     1890 2024-02-15 13:22:50.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/classification_miner.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.104776 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/
--rw-rw-rw-   0        0        0      910 2024-02-16 09:57:43.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.119818 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/
--rw-rw-rw-   0        0        0     1559 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/__init__.py
--rw-rw-rw-   0        0        0     3177 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/add_sequence_path_candidate.py
--rw-rw-rw-   0        0        0     5894 2024-02-15 13:20:01.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/candidate.py
--rw-rw-rw-   0        0        0     1780 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/candidate_queue.py
--rw-rw-rw-   0        0        0      859 2024-02-15 13:20:04.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/not_applicable_error.py
--rw-rw-rw-   0        0        0     5661 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/remove_chain_candidate.py
--rw-rw-rw-   0        0        0     2802 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/remove_edge_candidate.py
--rw-rw-rw-   0        0        0     7082 2024-02-16 09:58:21.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/consequence.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.132548 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/
--rw-rw-rw-   0        0        0     1520 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/__init__.py
--rw-rw-rw-   0        0        0     1433 2024-02-15 13:20:24.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/abstract.py
--rw-rw-rw-   0        0        0     1867 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/oracle.py
--rw-rw-rw-   0        0        0     2485 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/sequence_alignment_no_mdl.py
--rw-rw-rw-   0        0        0     6188 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/sequence_bottom_up.py
--rw-rw-rw-   0        0        0    10241 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/sequence_top_down.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.143388 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/
--rw-rw-rw-   0        0        0     1162 2024-02-15 13:18:38.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/__init__.py
--rw-rw-rw-   0        0        0    10680 2024-02-15 13:12:21.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/adversarial_lstm.py
--rw-rw-rw-   0        0        0    11062 2024-02-16 07:46:39.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/base_lstm.py
--rw-rw-rw-   0        0        0     1290 2024-02-15 13:18:45.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/batch_generator.py
--rw-rw-rw-   0        0        0     1856 2024-02-15 13:18:49.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/callbacks.py
--rw-rw-rw-   0        0        0     4521 2024-02-15 13:50:00.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/plain_lstm.py
--rw-rw-rw-   0        0        0     9991 2024-02-15 13:47:54.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/dats.py
--rw-rw-rw-   0        0        0     5088 2024-02-15 13:47:52.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/event_classifier.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.174418 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/
--rw-rw-rw-   0        0        0     1978 2024-02-15 13:21:21.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/__init__.py
--rw-rw-rw-   0        0        0     4647 2024-02-15 13:21:25.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/append_rule.py
--rw-rw-rw-   0        0        0     4902 2024-02-15 13:36:59.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/append_subsequence.py
--rw-rw-rw-   0        0        0     1179 2024-02-15 13:21:33.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/blackbox.py
--rw-rw-rw-   0        0        0     1789 2024-02-15 13:21:36.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/classification_rule.py
--rw-rw-rw-   0        0        0    10007 2024-02-15 13:21:40.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/event_flow_graph_rule.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.176390 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/export/
--rw-rw-rw-   0        0        0      811 2024-02-15 13:21:17.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/export/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.178393 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/export/html/
--rw-rw-rw-   0        0        0     6200 2024-02-15 13:20:58.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/export/html/error_highlighter.py
--rw-rw-rw-   0        0        0    10539 2024-02-15 13:21:44.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/if_then_else.py
--rw-rw-rw-   0        0        0   955134 2024-02-15 13:31:14.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/list_of_rules.cpp
--rw-rw-rw-   0        0        0     9282 2024-02-15 13:21:48.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/list_of_rules.pyx
--rw-rw-rw-   0        0        0   622490 2024-02-15 17:13:57.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/mdl.cpp
--rw-rw-rw-   0        0        0    13713 2024-02-15 17:13:41.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/mdl.pyx
--rw-rw-rw-   0        0        0   528761 2024-02-15 13:31:14.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/rule.cpp
--rw-rw-rw-   0        0        0     5891 2024-02-15 13:22:20.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/rule.pyx
--rw-rw-rw-   0        0        0     1964 2024-02-15 13:21:55.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/rule_literal.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.185080 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/window_classifier/
--rw-rw-rw-   0        0        0      927 2024-02-15 13:22:36.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/window_classifier/__init__.py
--rw-rw-rw-   0        0        0     3516 2024-02-15 13:22:41.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/window_classifier/window_classifier.py
--rw-rw-rw-   0        0        0     3301 2024-02-15 13:22:47.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/window_classifier/window_rule.py
--rw-rw-rw-   0        0        0     1943 2024-02-15 13:30:04.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/dataset_splitting_miner.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.188107 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/multilabel/
--rw-rw-rw-   0        0        0      811 2024-02-15 13:24:05.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/multilabel/__init__.py
--rw-rw-rw-   0        0        0     2769 2024-02-15 13:24:08.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/multilabel/evaluation.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.194024 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/multilabel/rules/
--rw-rw-rw-   0        0        0      175 2021-06-11 11:30:01.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/multilabel/rules/__init__.py
--rw-rw-rw-   0        0        0      770 2021-06-11 11:30:01.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/multilabel/rules/output_fixed_set_rule.py
--rw-rw-rw-   0        0        0      800 2021-06-11 11:30:01.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/multilabel/rules/rule.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.196782 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.199829 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/deep_generator/
--rw-rw-rw-   0        0        0      923 2024-02-15 13:24:19.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/deep_generator/__init__.py
--rw-rw-rw-   0        0        0    21271 2024-02-15 13:29:05.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/deep_generator/deep_generator.py
--rw-rw-rw-   0        0        0     1932 2024-02-15 13:29:54.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/eventlog_iterator.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.203807 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/irons/
--rw-rw-rw-   0        0        0       84 2021-05-26 13:05:26.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/irons/__init__.py
--rw-rw-rw-   0        0        0    10040 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/irons/irons.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.209807 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/trivial/
--rw-rw-rw-   0        0        0     1194 2024-02-15 13:29:41.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/trivial/__init__.py
--rw-rw-rw-   0        0        0     1405 2024-02-15 13:29:46.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/trivial/majority_event_predictor.py
--rw-rw-rw-   0        0        0     2472 2024-02-15 13:29:50.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/trivial/prefix_aware_majority_predictor.py
-drwxrwxrwx   0        0        0        0 2024-02-16 11:54:44.211806 prolothar-rule-mining-3.0.1/prolothar_rule_mining.egg-info/
--rw-rw-rw-   0        0        0     4057 2024-02-16 11:54:36.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10459 2024-02-16 11:54:43.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-16 11:54:36.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-16 10:44:18.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      117 2024-02-16 11:54:36.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-02-16 11:54:36.000000 prolothar-rule-mining-3.0.1/prolothar_rule_mining.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       78 2024-02-14 15:19:38.000000 prolothar-rule-mining-3.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       70 2024-02-15 11:01:58.000000 prolothar-rule-mining-3.0.1/requirements-dev.txt
--rw-rw-rw-   0        0        0      193 2024-02-15 13:49:32.000000 prolothar-rule-mining-3.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-02-16 11:54:44.215807 prolothar-rule-mining-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0     4174 2024-02-16 11:46:16.000000 prolothar-rule-mining-3.0.1/setup.py
--rw-rw-rw-   0        0        0        5 2024-02-16 11:52:49.000000 prolothar-rule-mining-3.0.1/version.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.810416 prolothar-rule-mining-3.0.2/
+-rw-rw-rw-   0        0        0    35821 2024-02-14 09:05:22.000000 prolothar-rule-mining-3.0.2/LICENSE
+-rw-rw-rw-   0        0        0      538 2024-02-16 11:53:11.000000 prolothar-rule-mining-3.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4227 2024-04-13 07:34:32.808416 prolothar-rule-mining-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3553 2024-04-13 07:25:00.000000 prolothar-rule-mining-3.0.2/README.md
+-rw-rw-rw-   0        0        0   105071 2024-02-15 13:38:27.000000 prolothar-rule-mining-3.0.2/coverage.xml
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.256735 prolothar-rule-mining-3.0.2/prolothar_rule_mining/
+-rw-rw-rw-   0        0        0      811 2024-02-15 13:30:07.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.337152 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/
+-rw-rw-rw-   0        0        0        0 2021-06-25 09:04:07.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/__init__.py
+-rw-rw-rw-   0        0        0  2312414 2024-04-13 07:34:09.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/conditions.cpp
+-rw-rw-rw-   0        0        0     1398 2024-04-13 07:29:55.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/conditions.pxd
+-rw-rw-rw-   0        0        0    22659 2024-02-15 13:12:21.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/conditions.pyx
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.344152 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/converter/
+-rw-rw-rw-   0        0        0     3068 2024-02-15 13:12:21.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/converter/eventflow_graph_to_pm4py_petrinet_converter.py
+-rw-rw-rw-   0        0        0     2603 2024-02-15 13:12:30.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/converter/sequence_to_class_dataset_converter.py
+-rw-rw-rw-   0        0        0     2016 2024-02-15 13:12:33.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/converter/sequence_to_multilabel_dataset_converter.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.354154 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/dataset_generator/
+-rw-rw-rw-   0        0        0     1120 2024-02-15 13:12:37.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/dataset_generator/__init__.py
+-rw-rw-rw-   0        0        0     4529 2024-02-15 13:12:46.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/dataset_generator/classification.py
+-rw-rw-rw-   0        0        0    17267 2024-02-15 13:12:49.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/dataset_generator/data_to_sequence.py
+-rw-rw-rw-   0        0        0     5270 2024-02-15 13:12:21.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/dataset_generator/dataset_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.379153 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/
+-rw-rw-rw-   0        0        0      881 2024-02-15 13:15:22.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/__init__.pxd
+-rw-rw-rw-   0        0        0     1089 2024-02-15 13:15:25.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.464155 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/
+-rw-rw-rw-   0        0        0        0 2021-06-25 09:04:07.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/__init__.py
+-rw-rw-rw-   0        0        0   342233 2024-04-13 07:34:09.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/a_star.cpp
+-rw-rw-rw-   0        0        0     2151 2024-02-15 13:14:07.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/a_star.pyx
+-rw-rw-rw-   0        0        0   671837 2024-04-13 07:34:10.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/alignment.cpp
+-rw-rw-rw-   0        0        0     1328 2024-02-15 13:13:41.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/alignment.pxd
+-rw-rw-rw-   0        0        0     2594 2024-02-15 13:13:45.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/alignment.pyx
+-rw-rw-rw-   0        0        0   382726 2024-04-13 07:34:10.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/alignment_finder.cpp
+-rw-rw-rw-   0        0        0      863 2024-02-15 13:13:08.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/alignment_finder.pxd
+-rw-rw-rw-   0        0        0     1451 2024-02-15 13:13:32.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/alignment_finder.pyx
+-rw-rw-rw-   0        0        0     2464 2024-02-15 13:13:50.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/beam_search.py
+-rw-rw-rw-   0        0        0     2515 2024-02-15 13:13:55.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/greedy_beam_search.py
+-rw-rw-rw-   0        0        0     3861 2024-02-15 13:14:00.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/greedy_shortest_path.py
+-rw-rw-rw-   0        0        0   797186 2024-04-13 07:34:10.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/heuristics.cpp
+-rw-rw-rw-   0        0        0     8191 2024-02-15 13:14:13.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/heuristics.pyx
+-rw-rw-rw-   0        0        0   599746 2024-04-13 07:34:10.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/partial_alignment.cpp
+-rw-rw-rw-   0        0        0     4847 2024-02-15 13:14:22.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/partial_alignment.pyx
+-rw-rw-rw-   0        0        0  1334535 2024-04-13 07:34:10.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/path_enumeration.cpp
+-rw-rw-rw-   0        0        0     5945 2024-02-15 13:14:28.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/path_enumeration.pyx
+-rw-rw-rw-   0        0        0     3092 2024-02-15 13:14:32.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/petrinet.py
+-rw-rw-rw-   0        0        0     3093 2024-02-15 13:14:36.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/sync_or_log_only.py
+-rw-rw-rw-   0        0        0     2509 2024-02-15 13:15:29.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/caching.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.475154 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/cover/
+-rw-rw-rw-   0        0        0     1458 2024-02-15 13:14:42.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/cover/__init__.py
+-rw-rw-rw-   0        0        0     8167 2024-02-15 13:14:50.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/cover/cover.py
+-rw-rw-rw-   0        0        0     4829 2024-02-15 13:14:47.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/cover/cover_computer.py
+-rw-rw-rw-   0        0        0     2428 2024-02-15 13:14:53.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/cover/model_code_counter.py
+-rw-rw-rw-   0        0        0     1613 2024-02-15 13:15:33.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/edge.py
+-rw-rw-rw-   0        0        0    23288 2024-02-16 10:10:05.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/graph.py
+-rw-rw-rw-   0        0        0   438653 2024-04-13 07:34:11.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/node.cpp
+-rw-rw-rw-   0        0        0      156 2021-06-25 09:04:07.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/node.pxd
+-rw-rw-rw-   0        0        0     2249 2024-02-15 13:15:44.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/node.pyx
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.483347 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/router/
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.492353 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/router/learning/
+-rw-rw-rw-   0        0        0     1062 2024-02-15 13:15:00.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/router/learning/__init__.py
+-rw-rw-rw-   0        0        0     2606 2024-02-15 13:15:03.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/router/learning/oracle_router_learner.py
+-rw-rw-rw-   0        0        0     2841 2024-02-15 13:15:06.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/router/learning/rule_classifier_router_learner.py
+-rw-rw-rw-   0        0        0     2723 2024-02-15 13:15:10.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/router/oracle_router.py
+-rw-rw-rw-   0        0        0     1085 2024-02-15 13:15:14.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/router/router.py
+-rw-rw-rw-   0        0        0     1707 2024-02-15 13:15:18.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/router/ruled_router.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.544351 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/
+-rw-rw-rw-   0        0        0      811 2024-02-15 13:30:01.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.546350 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/
+-rw-rw-rw-   0        0        0      811 2024-02-15 13:18:29.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.560351 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/knn/
+-rw-rw-rw-   0        0        0      894 2024-02-15 13:16:22.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/knn/__init__.py
+-rw-rw-rw-   0        0        0     2859 2024-02-16 08:41:33.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/knn/knn.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.571350 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/naive_bayes/
+-rw-rw-rw-   0        0        0     1057 2024-02-15 13:16:38.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/naive_bayes/__init__.py
+-rw-rw-rw-   0        0        0     3521 2024-02-15 13:12:21.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/naive_bayes/categorical_naive_bayes.py
+-rw-rw-rw-   0        0        0     2885 2024-02-15 13:12:21.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/naive_bayes/mixed_naive_bayes.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.578350 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/
+-rw-rw-rw-   0        0        0      914 2024-02-15 13:17:30.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/__init__.py
+-rw-rw-rw-   0        0        0     2672 2024-02-15 13:17:40.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/candidate.py
+-rw-rw-rw-   0        0        0     5265 2024-02-15 13:12:21.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/reliable_rule_miner.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.593350 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/strategy/
+-rw-rw-rw-   0        0        0   895366 2024-04-13 07:34:11.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/strategy/abstract.cpp
+-rw-rw-rw-   0        0        0    13305 2024-02-15 13:17:07.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/strategy/abstract.pyx
+-rw-rw-rw-   0        0        0     6866 2024-02-15 13:17:10.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/strategy/beam_search.py
+-rw-rw-rw-   0        0        0     4489 2024-02-15 13:17:21.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/strategy/best_first.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.618351 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/
+-rw-rw-rw-   0        0        0     1396 2024-02-15 13:18:02.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/__init__.py
+-rw-rw-rw-   0        0        0      962 2024-02-15 13:17:59.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/class_output_exception.py
+-rw-rw-rw-   0        0        0     2436 2024-02-15 13:18:06.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/first_firing_rule_model.py
+-rw-rw-rw-   0        0        0     4227 2024-02-15 13:18:10.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/if_then_else_rule.py
+-rw-rw-rw-   0        0        0     3811 2024-02-15 13:18:13.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/list_of_rules.py
+-rw-rw-rw-   0        0        0     2316 2024-02-15 13:18:17.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/return_class_rule.py
+-rw-rw-rw-   0        0        0     1893 2024-02-15 13:18:20.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/rule.py
+-rw-rw-rw-   0        0        0     5337 2024-02-16 09:30:36.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/sklearn.py
+-rw-rw-rw-   0        0        0     1931 2024-02-15 13:18:27.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/voting_class_rule.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.628349 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/
+-rw-rw-rw-   0        0        0     1890 2024-02-15 13:22:50.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/classification_miner.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.634353 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/
+-rw-rw-rw-   0        0        0      910 2024-02-16 09:57:43.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.660350 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/
+-rw-rw-rw-   0        0        0     1559 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/__init__.py
+-rw-rw-rw-   0        0        0     3177 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/add_sequence_path_candidate.py
+-rw-rw-rw-   0        0        0     5894 2024-02-15 13:20:01.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/candidate.py
+-rw-rw-rw-   0        0        0     1780 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/candidate_queue.py
+-rw-rw-rw-   0        0        0      859 2024-02-15 13:20:04.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/not_applicable_error.py
+-rw-rw-rw-   0        0        0     5661 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/remove_chain_candidate.py
+-rw-rw-rw-   0        0        0     2802 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/remove_edge_candidate.py
+-rw-rw-rw-   0        0        0     7082 2024-02-16 09:58:21.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/consequence.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.683352 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/
+-rw-rw-rw-   0        0        0     1520 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/__init__.py
+-rw-rw-rw-   0        0        0     1433 2024-02-15 13:20:24.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/abstract.py
+-rw-rw-rw-   0        0        0     1867 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/oracle.py
+-rw-rw-rw-   0        0        0     2485 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/sequence_alignment_no_mdl.py
+-rw-rw-rw-   0        0        0     6188 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/sequence_bottom_up.py
+-rw-rw-rw-   0        0        0    10241 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/sequence_top_down.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.701416 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/
+-rw-rw-rw-   0        0        0     1162 2024-02-15 13:18:38.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/__init__.py
+-rw-rw-rw-   0        0        0    10680 2024-02-15 13:12:21.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/adversarial_lstm.py
+-rw-rw-rw-   0        0        0    11062 2024-02-16 07:46:39.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/base_lstm.py
+-rw-rw-rw-   0        0        0     1290 2024-02-15 13:18:45.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/batch_generator.py
+-rw-rw-rw-   0        0        0     1856 2024-02-15 13:18:49.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/callbacks.py
+-rw-rw-rw-   0        0        0     4521 2024-02-15 13:50:00.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/plain_lstm.py
+-rw-rw-rw-   0        0        0     9991 2024-02-15 13:47:54.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/dats.py
+-rw-rw-rw-   0        0        0     5088 2024-02-15 13:47:52.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/event_classifier.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.751417 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/
+-rw-rw-rw-   0        0        0     1978 2024-02-15 13:21:21.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/__init__.py
+-rw-rw-rw-   0        0        0     4647 2024-02-15 13:21:25.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/append_rule.py
+-rw-rw-rw-   0        0        0     4902 2024-02-15 13:36:59.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/append_subsequence.py
+-rw-rw-rw-   0        0        0     1179 2024-02-15 13:21:33.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/blackbox.py
+-rw-rw-rw-   0        0        0     1789 2024-02-15 13:21:36.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/classification_rule.py
+-rw-rw-rw-   0        0        0    10007 2024-02-15 13:21:40.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/event_flow_graph_rule.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.754416 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/export/
+-rw-rw-rw-   0        0        0      811 2024-02-15 13:21:17.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/export/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.758415 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/export/html/
+-rw-rw-rw-   0        0        0     6200 2024-02-15 13:20:58.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/export/html/error_highlighter.py
+-rw-rw-rw-   0        0        0    10539 2024-02-15 13:21:44.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/if_then_else.py
+-rw-rw-rw-   0        0        0   955676 2024-04-13 07:34:11.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/list_of_rules.cpp
+-rw-rw-rw-   0        0        0     9282 2024-02-15 13:21:48.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/list_of_rules.pyx
+-rw-rw-rw-   0        0        0   622960 2024-04-13 07:34:11.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/mdl.cpp
+-rw-rw-rw-   0        0        0    13713 2024-02-15 17:13:41.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/mdl.pyx
+-rw-rw-rw-   0        0        0   529231 2024-04-13 07:34:11.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/rule.cpp
+-rw-rw-rw-   0        0        0     5891 2024-02-15 13:22:20.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/rule.pyx
+-rw-rw-rw-   0        0        0     1964 2024-02-15 13:21:55.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/rule_literal.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.765414 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/window_classifier/
+-rw-rw-rw-   0        0        0      927 2024-02-15 13:22:36.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/window_classifier/__init__.py
+-rw-rw-rw-   0        0        0     3516 2024-02-15 13:22:41.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/window_classifier/window_classifier.py
+-rw-rw-rw-   0        0        0     3301 2024-02-15 13:22:47.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/window_classifier/window_rule.py
+-rw-rw-rw-   0        0        0     1943 2024-02-15 13:30:04.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/dataset_splitting_miner.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.770416 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/multilabel/
+-rw-rw-rw-   0        0        0      811 2024-02-15 13:24:05.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/multilabel/__init__.py
+-rw-rw-rw-   0        0        0     2769 2024-02-15 13:24:08.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/multilabel/evaluation.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.778415 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/multilabel/rules/
+-rw-rw-rw-   0        0        0      175 2021-06-11 11:30:01.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/multilabel/rules/__init__.py
+-rw-rw-rw-   0        0        0      770 2021-06-11 11:30:01.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/multilabel/rules/output_fixed_set_rule.py
+-rw-rw-rw-   0        0        0      800 2021-06-11 11:30:01.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/multilabel/rules/rule.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.781417 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.786417 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/deep_generator/
+-rw-rw-rw-   0        0        0      923 2024-02-15 13:24:19.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/deep_generator/__init__.py
+-rw-rw-rw-   0        0        0    21271 2024-02-15 13:29:05.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/deep_generator/deep_generator.py
+-rw-rw-rw-   0        0        0     1932 2024-02-15 13:29:54.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/eventlog_iterator.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.794416 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/irons/
+-rw-rw-rw-   0        0        0       84 2021-05-26 13:05:26.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/irons/__init__.py
+-rw-rw-rw-   0        0        0    10040 2024-02-16 09:58:08.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/irons/irons.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.804417 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/trivial/
+-rw-rw-rw-   0        0        0     1194 2024-02-15 13:29:41.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/trivial/__init__.py
+-rw-rw-rw-   0        0        0     1405 2024-02-15 13:29:46.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/trivial/majority_event_predictor.py
+-rw-rw-rw-   0        0        0     2472 2024-02-15 13:29:50.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/trivial/prefix_aware_majority_predictor.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:34:32.807417 prolothar-rule-mining-3.0.2/prolothar_rule_mining.egg-info/
+-rw-rw-rw-   0        0        0     4227 2024-04-13 07:34:22.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10764 2024-04-13 07:34:32.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 07:34:22.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-13 07:34:11.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      117 2024-04-13 07:34:22.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-13 07:34:22.000000 prolothar-rule-mining-3.0.2/prolothar_rule_mining.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       98 2024-04-13 07:31:14.000000 prolothar-rule-mining-3.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       70 2024-02-15 11:01:58.000000 prolothar-rule-mining-3.0.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0      193 2024-02-15 13:49:32.000000 prolothar-rule-mining-3.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 07:34:32.810416 prolothar-rule-mining-3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     4127 2024-04-13 07:11:13.000000 prolothar-rule-mining-3.0.2/setup.py
+-rw-rw-rw-   0        0        0        5 2024-04-13 07:08:27.000000 prolothar-rule-mining-3.0.2/version.txt
```

### Comparing `prolothar-rule-mining-3.0.1/LICENSE` & `prolothar-rule-mining-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/MANIFEST.in` & `prolothar-rule-mining-3.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/PKG-INFO` & `prolothar-rule-mining-3.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: prolothar-rule-mining
-Version: 3.0.1
-Summary: algorithms for process mining and data mining on event sequences
-Home-page: https://gitlab.dillinger.de/KI/DataScience/processmining/prolothar-process-discovery
+Version: 3.0.2
+Summary: algorithms for prediction and rule mining on event sequences
+Home-page: https://github.com/shs-it/prolothar-rule-mining
 Author: Boris Wiegand
 Author-email: boris.wiegand@stahl-holding-saar.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyfim==6.28
@@ -105,16 +105,16 @@
 graph.plot()
 graph.plot(view=False, filepath='path_to_pdf')
 
 #get and print the classification rule at each node
 for node, router in rules_model.get_node_router_table().items():
     print('===============================')
     print(f'rule at node {node}')
-    print(node.get_rule())
-    # alternative: print(node.get_rule().to_html())
+    print(router.get_rule())
+    # alternative: print(router.get_rule().to_html())
 ```
 
 ## Development
 
 These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.
 
 ### Additional Prerequisites
@@ -130,16 +130,24 @@
 
 ```bash
 make test
 ```
 
 ### Deployment
 
+1. Change the version in version.txt
+2. Build and publish the package on pypi by
 ```bash
-make clean_package || make package && make publish
+make clean_package
+make package && make publish
+```
+3. Create and push a tag for this version by
+```bash
+git tag -a [version] -m "describe this version"
+git push --tags
 ```
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning.
 
 ## Authors
```

### Comparing `prolothar-rule-mining-3.0.1/README.md` & `prolothar-rule-mining-3.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -86,16 +86,16 @@
 graph.plot()
 graph.plot(view=False, filepath='path_to_pdf')
 
 #get and print the classification rule at each node
 for node, router in rules_model.get_node_router_table().items():
     print('===============================')
     print(f'rule at node {node}')
-    print(node.get_rule())
-    # alternative: print(node.get_rule().to_html())
+    print(router.get_rule())
+    # alternative: print(router.get_rule().to_html())
 ```
 
 ## Development
 
 These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.
 
 ### Additional Prerequisites
@@ -111,16 +111,24 @@
 
 ```bash
 make test
 ```
 
 ### Deployment
 
+1. Change the version in version.txt
+2. Build and publish the package on pypi by
 ```bash
-make clean_package || make package && make publish
+make clean_package
+make package && make publish
+```
+3. Create and push a tag for this version by
+```bash
+git tag -a [version] -m "describe this version"
+git push --tags
 ```
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning.
 
 ## Authors
```

### Comparing `prolothar-rule-mining-3.0.1/coverage.xml` & `prolothar-rule-mining-3.0.2/coverage.xml`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/conditions.cpp` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/conditions.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "language": "c++",
         "name": "prolothar_rule_mining.models.conditions",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -745,16 +775,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1098,15 +1133,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1185,15 +1220,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1284,32 +1319,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1473,15 +1491,15 @@
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "prolothar_rule_mining\\\\models\\\\conditions.pyx",
   "<stringsource>",
   "prolothar_rule_mining\\\\models\\\\conditions.pxd",
-  ".venv\\\\Lib\\\\site-packages\\\\prolothar_common\\\\models\\\\dataset\\\\instance.pxd",
+  "instance.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
@@ -1594,15 +1612,15 @@
 };
 
 
 /* "prolothar_rule_mining/models/conditions.pxd":23
  *     cpdef float compute_mdl(self, int nr_of_attributes)
  * 
  * cdef class AttributeCondition(Condition):             # <<<<<<<<<<<<<<
- *     cdef public attribute
+ *     cdef public object attribute
  *     cdef public str operator_symbol
  */
 struct __pyx_obj_21prolothar_rule_mining_6models_10conditions_AttributeCondition {
   struct __pyx_obj_21prolothar_rule_mining_6models_10conditions_Condition __pyx_base;
   PyObject *attribute;
   PyObject *operator_symbol;
   PyObject *value;
@@ -2727,30 +2745,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_8
-#define __PYX_HAVE_RT_ImportType_proto_3_0_8
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_8 {
-   __Pyx_ImportType_CheckSize_Error_3_0_8 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_8 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_8 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
 #if PY_MAJOR_VERSION >= 3
 static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
 #endif
@@ -10711,17 +10729,17 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "prolothar_rule_mining/models/conditions.pxd":24
  * 
  * cdef class AttributeCondition(Condition):
- *     cdef public attribute             # <<<<<<<<<<<<<<
+ *     cdef public object attribute             # <<<<<<<<<<<<<<
  *     cdef public str operator_symbol
- *     cdef public value
+ *     cdef public object value
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_21prolothar_rule_mining_6models_10conditions_18AttributeCondition_9attribute_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_21prolothar_rule_mining_6models_10conditions_18AttributeCondition_9attribute_1__get__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
@@ -10811,17 +10829,17 @@
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "prolothar_rule_mining/models/conditions.pxd":25
  * cdef class AttributeCondition(Condition):
- *     cdef public attribute
+ *     cdef public object attribute
  *     cdef public str operator_symbol             # <<<<<<<<<<<<<<
- *     cdef public value
+ *     cdef public object value
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_21prolothar_rule_mining_6models_10conditions_18AttributeCondition_15operator_symbol_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_21prolothar_rule_mining_6models_10conditions_18AttributeCondition_15operator_symbol_1__get__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
@@ -10924,17 +10942,17 @@
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "prolothar_rule_mining/models/conditions.pxd":26
- *     cdef public attribute
+ *     cdef public object attribute
  *     cdef public str operator_symbol
- *     cdef public value             # <<<<<<<<<<<<<<
+ *     cdef public object value             # <<<<<<<<<<<<<<
  * 
  *     cdef bint check_value(self, tested_value)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_21prolothar_rule_mining_6models_10conditions_18AttributeCondition_5value_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_21prolothar_rule_mining_6models_10conditions_18AttributeCondition_5value_1__get__(PyObject *__pyx_v_self) {
@@ -37270,24 +37288,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct__genexpr *__pyx_freelist_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct__genexpr[8];
 static int __pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct__genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct__genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct__genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct__genexpr)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct__genexpr[--__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct__genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct__genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -37307,15 +37327,15 @@
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_c);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct__genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct__genexpr)))) {
     __pyx_freelist_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct__genexpr[__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct__genexpr++] = ((struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct__genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -37433,24 +37453,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_1_genexpr *__pyx_freelist_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_1_genexpr[8];
 static int __pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_1_genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_1_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_1_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_1_genexpr)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_1_genexpr[--__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_1_genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_1_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -37470,15 +37492,15 @@
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_c);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_1_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_1_genexpr)))) {
     __pyx_freelist_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_1_genexpr[__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_1_genexpr++] = ((struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_1_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -37596,24 +37618,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_2_to_bal *__pyx_freelist_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_2_to_bal[8];
 static int __pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_2_to_bal = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_2_to_bal(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_2_to_bal > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_2_to_bal)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_2_to_bal[--__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_2_to_bal];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_2_to_bal));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -37636,15 +37660,15 @@
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_attribute_formatter);
   Py_CLEAR(p->__pyx_v_categorical_value_formatter);
   Py_CLEAR(p->__pyx_v_join_operator_formatter);
   Py_CLEAR(p->__pyx_v_numerical_value_formatter);
   Py_CLEAR(p->__pyx_v_operator_formatter);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_2_to_bal < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_2_to_bal)))) {
     __pyx_freelist_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_2_to_bal[__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_2_to_bal++] = ((struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_2_to_bal *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -37793,24 +37817,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_3_genexpr *__pyx_freelist_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_3_genexpr[8];
 static int __pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_3_genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_3_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_3_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_3_genexpr)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_3_genexpr[--__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_3_genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_3_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -37831,15 +37857,15 @@
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_outer_scope);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_condition);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_3_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_3_genexpr)))) {
     __pyx_freelist_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_3_genexpr[__pyx_freecount_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_3_genexpr++] = ((struct __pyx_obj_21prolothar_rule_mining_6models_10conditions___pyx_scope_struct_3_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -39699,23 +39725,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("prolothar_common.models.dataset.instance"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_16prolothar_common_6models_7dataset_8instance_Instance = __Pyx_ImportType_3_0_8(__pyx_t_1, "prolothar_common.models.dataset.instance", "Instance", sizeof(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_Instance), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_Instance),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_16prolothar_common_6models_7dataset_8instance_Instance) __PYX_ERR(3, 18, __pyx_L1_error)
+  __pyx_ptype_16prolothar_common_6models_7dataset_8instance_Instance = __Pyx_ImportType_3_0_10(__pyx_t_1, "prolothar_common.models.dataset.instance", "Instance", sizeof(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_Instance), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_Instance),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_16prolothar_common_6models_7dataset_8instance_Instance) __PYX_ERR(3, 18, __pyx_L1_error)
   __pyx_vtabptr_16prolothar_common_6models_7dataset_8instance_Instance = (struct __pyx_vtabstruct_16prolothar_common_6models_7dataset_8instance_Instance*)__Pyx_GetVtable(__pyx_ptype_16prolothar_common_6models_7dataset_8instance_Instance); if (unlikely(!__pyx_vtabptr_16prolothar_common_6models_7dataset_8instance_Instance)) __PYX_ERR(3, 18, __pyx_L1_error)
-  __pyx_ptype_16prolothar_common_6models_7dataset_8instance_ClassificationInstance = __Pyx_ImportType_3_0_8(__pyx_t_1, "prolothar_common.models.dataset.instance", "ClassificationInstance", sizeof(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_ClassificationInstance), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_ClassificationInstance),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_16prolothar_common_6models_7dataset_8instance_ClassificationInstance) __PYX_ERR(3, 25, __pyx_L1_error)
+  __pyx_ptype_16prolothar_common_6models_7dataset_8instance_ClassificationInstance = __Pyx_ImportType_3_0_10(__pyx_t_1, "prolothar_common.models.dataset.instance", "ClassificationInstance", sizeof(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_ClassificationInstance), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_ClassificationInstance),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_16prolothar_common_6models_7dataset_8instance_ClassificationInstance) __PYX_ERR(3, 25, __pyx_L1_error)
   __pyx_vtabptr_16prolothar_common_6models_7dataset_8instance_ClassificationInstance = (struct __pyx_vtabstruct_16prolothar_common_6models_7dataset_8instance_ClassificationInstance*)__Pyx_GetVtable(__pyx_ptype_16prolothar_common_6models_7dataset_8instance_ClassificationInstance); if (unlikely(!__pyx_vtabptr_16prolothar_common_6models_7dataset_8instance_ClassificationInstance)) __PYX_ERR(3, 25, __pyx_L1_error)
-  __pyx_ptype_16prolothar_common_6models_7dataset_8instance_MultiLabelInstance = __Pyx_ImportType_3_0_8(__pyx_t_1, "prolothar_common.models.dataset.instance", "MultiLabelInstance", sizeof(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_MultiLabelInstance), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_MultiLabelInstance),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_16prolothar_common_6models_7dataset_8instance_MultiLabelInstance) __PYX_ERR(3, 31, __pyx_L1_error)
+  __pyx_ptype_16prolothar_common_6models_7dataset_8instance_MultiLabelInstance = __Pyx_ImportType_3_0_10(__pyx_t_1, "prolothar_common.models.dataset.instance", "MultiLabelInstance", sizeof(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_MultiLabelInstance), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_MultiLabelInstance),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_16prolothar_common_6models_7dataset_8instance_MultiLabelInstance) __PYX_ERR(3, 31, __pyx_L1_error)
   __pyx_vtabptr_16prolothar_common_6models_7dataset_8instance_MultiLabelInstance = (struct __pyx_vtabstruct_16prolothar_common_6models_7dataset_8instance_MultiLabelInstance*)__Pyx_GetVtable(__pyx_ptype_16prolothar_common_6models_7dataset_8instance_MultiLabelInstance); if (unlikely(!__pyx_vtabptr_16prolothar_common_6models_7dataset_8instance_MultiLabelInstance)) __PYX_ERR(3, 31, __pyx_L1_error)
-  __pyx_ptype_16prolothar_common_6models_7dataset_8instance_MultisetInstance = __Pyx_ImportType_3_0_8(__pyx_t_1, "prolothar_common.models.dataset.instance", "MultisetInstance", sizeof(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_MultisetInstance), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_MultisetInstance),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_16prolothar_common_6models_7dataset_8instance_MultisetInstance) __PYX_ERR(3, 37, __pyx_L1_error)
+  __pyx_ptype_16prolothar_common_6models_7dataset_8instance_MultisetInstance = __Pyx_ImportType_3_0_10(__pyx_t_1, "prolothar_common.models.dataset.instance", "MultisetInstance", sizeof(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_MultisetInstance), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_MultisetInstance),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_16prolothar_common_6models_7dataset_8instance_MultisetInstance) __PYX_ERR(3, 37, __pyx_L1_error)
   __pyx_vtabptr_16prolothar_common_6models_7dataset_8instance_MultisetInstance = (struct __pyx_vtabstruct_16prolothar_common_6models_7dataset_8instance_MultisetInstance*)__Pyx_GetVtable(__pyx_ptype_16prolothar_common_6models_7dataset_8instance_MultisetInstance); if (unlikely(!__pyx_vtabptr_16prolothar_common_6models_7dataset_8instance_MultisetInstance)) __PYX_ERR(3, 37, __pyx_L1_error)
-  __pyx_ptype_16prolothar_common_6models_7dataset_8instance_TargetSequenceInstance = __Pyx_ImportType_3_0_8(__pyx_t_1, "prolothar_common.models.dataset.instance", "TargetSequenceInstance", sizeof(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_TargetSequenceInstance), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_TargetSequenceInstance),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_16prolothar_common_6models_7dataset_8instance_TargetSequenceInstance) __PYX_ERR(3, 42, __pyx_L1_error)
+  __pyx_ptype_16prolothar_common_6models_7dataset_8instance_TargetSequenceInstance = __Pyx_ImportType_3_0_10(__pyx_t_1, "prolothar_common.models.dataset.instance", "TargetSequenceInstance", sizeof(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_TargetSequenceInstance), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_16prolothar_common_6models_7dataset_8instance_TargetSequenceInstance),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_16prolothar_common_6models_7dataset_8instance_TargetSequenceInstance) __PYX_ERR(3, 42, __pyx_L1_error)
   __pyx_vtabptr_16prolothar_common_6models_7dataset_8instance_TargetSequenceInstance = (struct __pyx_vtabstruct_16prolothar_common_6models_7dataset_8instance_TargetSequenceInstance*)__Pyx_GetVtable(__pyx_ptype_16prolothar_common_6models_7dataset_8instance_TargetSequenceInstance); if (unlikely(!__pyx_vtabptr_16prolothar_common_6models_7dataset_8instance_TargetSequenceInstance)) __PYX_ERR(3, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -44803,18 +44829,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_8
-#define __PYX_HAVE_RT_ImportType_3_0_8
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -44860,23 +44886,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_8 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_8 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -45996,15 +46022,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/conditions.pyx` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/conditions.pyx`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/converter/eventflow_graph_to_pm4py_petrinet_converter.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/converter/eventflow_graph_to_pm4py_petrinet_converter.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/converter/sequence_to_class_dataset_converter.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/converter/sequence_to_class_dataset_converter.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/converter/sequence_to_multilabel_dataset_converter.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/converter/sequence_to_multilabel_dataset_converter.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/dataset_generator/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/dataset_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/dataset_generator/classification.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/dataset_generator/classification.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/dataset_generator/data_to_sequence.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/dataset_generator/data_to_sequence.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/dataset_generator/dataset_generator.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/dataset_generator/dataset_generator.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/a_star.cpp` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/a_star.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "language": "c++",
         "name": "prolothar_rule_mining.models.event_flow_graph.alignment.a_star",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -745,16 +775,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1098,15 +1133,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1185,15 +1220,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1284,32 +1319,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -6647,15 +6665,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/a_star.pyx` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/a_star.pyx`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/alignment.cpp` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/alignment.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "language": "c++",
         "name": "prolothar_rule_mining.models.event_flow_graph.alignment.alignment",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -745,16 +775,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1098,15 +1133,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1185,15 +1220,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1284,32 +1319,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -2188,30 +2206,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_8
-#define __PYX_HAVE_RT_ImportType_proto_3_0_8
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_8 {
-   __Pyx_ImportType_CheckSize_Error_3_0_8 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_8 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_8 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* PyMethodNew.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
 static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
     PyObject *typesModule=NULL, *methodType=NULL, *result=NULL;
     CYTHON_UNUSED_VAR(typ);
@@ -8053,24 +8071,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__ *__pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__[8];
 static int __pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__ = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__ > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__[--__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -8089,15 +8109,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__ < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__)))) {
     __pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__[__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__++] = ((struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment___pyx_scope_struct____iter__ *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -8631,15 +8651,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("prolothar_rule_mining.models.event_flow_graph.node"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node = __Pyx_ImportType_3_0_8(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.node", "Node", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node = __Pyx_ImportType_3_0_10(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.node", "Node", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -12924,18 +12944,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_8
-#define __PYX_HAVE_RT_ImportType_3_0_8
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -12981,23 +13001,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_8 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_8 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -13883,15 +13903,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/alignment.pyx` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/alignment.pyx`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/alignment_finder.cpp` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/alignment_finder.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "language": "c++",
         "name": "prolothar_rule_mining.models.event_flow_graph.alignment.alignment_finder",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -745,16 +775,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1098,15 +1133,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1185,15 +1220,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1284,32 +1319,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -7664,15 +7682,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/alignment_finder.pyx` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/alignment_finder.pyx`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/beam_search.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/beam_search.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/greedy_beam_search.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/greedy_beam_search.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/greedy_shortest_path.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/greedy_shortest_path.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/heuristics.cpp` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/heuristics.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "language": "c++",
         "name": "prolothar_rule_mining.models.event_flow_graph.alignment.heuristics",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -745,16 +775,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1098,15 +1133,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1185,15 +1220,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1284,32 +1319,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -9296,24 +9314,26 @@
   __Pyx_XDECREF(__pyx_gb_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics_16MaximumHeuristic_8__call___2generator1);
   __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct__genexpr *__pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct__genexpr[8];
 static int __pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct__genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct__genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct__genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct__genexpr)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct__genexpr[--__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct__genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct__genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -9334,15 +9354,15 @@
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_parent);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct__genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct__genexpr)))) {
     __pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct__genexpr[__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct__genexpr++] = ((struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct__genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -9463,24 +9483,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_1___call__ *__pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_1___call__[8];
 static int __pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_1___call__ = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_1___call__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_1___call__ > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_1___call__)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_1___call__[--__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_1___call__];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_1___call__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -9501,15 +9523,15 @@
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_event_index);
   Py_CLEAR(p->__pyx_v_node);
   Py_CLEAR(p->__pyx_v_sequence);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_1___call__ < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_1___call__)))) {
     __pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_1___call__[__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_1___call__++] = ((struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_1___call__ *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -9640,24 +9662,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_2_genexpr *__pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_2_genexpr[8];
 static int __pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_2_genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_2_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_2_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_2_genexpr)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_2_genexpr[--__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_2_genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_2_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -9679,15 +9703,15 @@
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_outer_scope);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_heuristic);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_2_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_2_genexpr)))) {
     __pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_2_genexpr[__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_2_genexpr++] = ((struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_10heuristics___pyx_scope_struct_2_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -14810,15 +14834,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/heuristics.pyx` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/heuristics.pyx`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/partial_alignment.cpp` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/partial_alignment.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "language": "c++",
         "name": "prolothar_rule_mining.models.event_flow_graph.alignment.partial_alignment",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -745,16 +775,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1098,15 +1133,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1185,15 +1220,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1284,32 +1319,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -2062,30 +2080,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_8
-#define __PYX_HAVE_RT_ImportType_proto_3_0_8
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_8 {
-   __Pyx_ImportType_CheckSize_Error_3_0_8 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_8 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_8 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -6442,24 +6460,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_17partial_alignment___pyx_scope_struct__yield_neighbors *__pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_17partial_alignment___pyx_scope_struct__yield_neighbors[8];
 static int __pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_17partial_alignment___pyx_scope_struct__yield_neighbors = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_17partial_alignment___pyx_scope_struct__yield_neighbors(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_17partial_alignment___pyx_scope_struct__yield_neighbors > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_17partial_alignment___pyx_scope_struct__yield_neighbors)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_17partial_alignment___pyx_scope_struct__yield_neighbors[--__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_17partial_alignment___pyx_scope_struct__yield_neighbors];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_17partial_alignment___pyx_scope_struct__yield_neighbors));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -6485,15 +6505,15 @@
   Py_CLEAR(p->__pyx_v_heuristic);
   Py_CLEAR(p->__pyx_v_model_move_cost);
   Py_CLEAR(p->__pyx_v_next_event);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_v_sequence);
   Py_CLEAR(p->__pyx_v_sink);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_17partial_alignment___pyx_scope_struct__yield_neighbors < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_17partial_alignment___pyx_scope_struct__yield_neighbors)))) {
     __pyx_freelist_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_17partial_alignment___pyx_scope_struct__yield_neighbors[__pyx_freecount_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_17partial_alignment___pyx_scope_struct__yield_neighbors++] = ((struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_17partial_alignment___pyx_scope_struct__yield_neighbors *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -6921,21 +6941,21 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("prolothar_rule_mining.models.event_flow_graph.node"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node = __Pyx_ImportType_3_0_8(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.node", "Node", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node = __Pyx_ImportType_3_0_10(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.node", "Node", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("prolothar_rule_mining.models.event_flow_graph.alignment.alignment"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move = __Pyx_ImportType_3_0_8(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.alignment.alignment", "Move", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move) __PYX_ERR(3, 19, __pyx_L1_error)
+  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move = __Pyx_ImportType_3_0_10(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.alignment.alignment", "Move", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move) __PYX_ERR(3, 19, __pyx_L1_error)
   __pyx_vtabptr_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move = (struct __pyx_vtabstruct_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move*)__Pyx_GetVtable(__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move); if (unlikely(!__pyx_vtabptr_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move)) __PYX_ERR(3, 19, __pyx_L1_error)
-  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment = __Pyx_ImportType_3_0_8(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.alignment.alignment", "Alignment", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment) __PYX_ERR(3, 27, __pyx_L1_error)
+  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment = __Pyx_ImportType_3_0_10(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.alignment.alignment", "Alignment", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment) __PYX_ERR(3, 27, __pyx_L1_error)
   __pyx_vtabptr_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment = (struct __pyx_vtabstruct_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment*)__Pyx_GetVtable(__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment); if (unlikely(!__pyx_vtabptr_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment)) __PYX_ERR(3, 27, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -9523,18 +9543,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_8
-#define __PYX_HAVE_RT_ImportType_3_0_8
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -9580,23 +9600,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_8 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_8 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -10689,15 +10709,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/partial_alignment.pyx` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/partial_alignment.pyx`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/path_enumeration.cpp` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/path_enumeration.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "language": "c++",
         "name": "prolothar_rule_mining.models.event_flow_graph.alignment.path_enumeration",
@@ -34,18 +34,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -129,14 +129,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -190,14 +192,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -251,60 +255,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -387,14 +414,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -746,16 +776,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1099,15 +1134,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1186,15 +1221,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1289,32 +1324,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1477,15 +1495,15 @@
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "prolothar_rule_mining\\\\models\\\\event_flow_graph\\\\alignment\\\\path_enumeration.pyx",
   "<stringsource>",
-  ".venv\\\\Lib\\\\site-packages\\\\prolothar_common\\\\levenshtein.pxd",
+  "levenshtein.pxd",
   "prolothar_rule_mining\\\\models\\\\event_flow_graph\\\\node.pxd",
   "prolothar_rule_mining\\\\models\\\\event_flow_graph\\\\alignment\\\\alignment.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
@@ -1634,15 +1652,15 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation;
 struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node;
 struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move;
 struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment;
 struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder;
 struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration;
-struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e;
+struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 struct __pyx_opt_args_16prolothar_common_11levenshtein_compute_cost_matrix;
 
 /* "prolothar_common/levenshtein.pxd":18
@@ -1769,20 +1787,20 @@
   struct __pyx_vtabstruct_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration *__pyx_vtab;
   PyObject *all_paths;
 };
 
 
 /* "cfunc.to_py":66
  * 
- * @cname("__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e")
- * cdef object __Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e((int, int)  (*f)(EditOperation) except *):             # <<<<<<<<<<<<<<
+ * @cname("__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e")
+ * cdef object __Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e((int, int)  (*f)(EditOperation) except *):             # <<<<<<<<<<<<<<
  *     def wrap(EditOperation e):
  *         """wrap(e: 'EditOperation') -> '(int, int) '"""
  */
-struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e {
+struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e {
   PyObject_HEAD
   __pyx_ctuple_int__and_int (*__pyx_v_f)(struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation *);
 };
 
 
 /* "View.MemoryView":114
  * @cython.collection_type("sequence")
@@ -2852,30 +2870,30 @@
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_8
-#define __PYX_HAVE_RT_ImportType_proto_3_0_8
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_8 {
-   __Pyx_ImportType_CheckSize_Error_3_0_8 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_8 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_8 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* ValidateBasesTuple.proto */
 #if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
 static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases);
 #endif
 
@@ -3054,15 +3072,15 @@
 #endif
 
 /* CheckBinaryVersion.proto */
 static unsigned long __Pyx_get_runtime_version(void);
 static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction_3_0_8(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_3_0_10(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self); /* proto*/
 static char *__pyx_memoryview_get_item_pointer(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index); /* proto*/
@@ -3087,26 +3105,27 @@
 /* Module declarations from "prolothar_rule_mining.models.event_flow_graph" */
 
 /* Module declarations from "prolothar_rule_mining.models.event_flow_graph.alignment.alignment" */
 
 /* Module declarations from "prolothar_rule_mining.models.event_flow_graph.alignment.alignment_finder" */
 
 /* Module declarations from "prolothar_rule_mining.models.event_flow_graph.alignment.path_enumeration" */
+static PyObject *__pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py = 0;
 static PyObject *__pyx_collections_abc_Sequence = 0;
 static PyObject *generic = 0;
 static PyObject *strided = 0;
 static PyObject *indirect = 0;
 static PyObject *contiguous = 0;
 static PyObject *indirect_contiguous = 0;
 static int __pyx_memoryview_thread_locks_used;
 static PyThread_type_lock __pyx_memoryview_thread_locks[8];
 static __pyx_ctuple_int__and_int __pyx_f_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_edit_operation_sort(struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation *); /*proto*/
 static PyObject *__pyx_f_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration___pyx_unpickle_PathEnumeration__set_state(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration *, PyObject *); /*proto*/
-static PyObject *__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e(__pyx_ctuple_int__and_int (*)(struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation *)); /*proto*/
-static PyObject *__Pyx_Enum_bca7cc__enum__dunderpyx_t_16prolothar_common_11levenshtein_EditOperationType__etc_to_py(enum __pyx_t_16prolothar_common_11levenshtein_EditOperationType); /*proto*/
+static PyObject *__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e(__pyx_ctuple_int__and_int (*)(struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation *)); /*proto*/
+static PyObject *__Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py(enum __pyx_t_16prolothar_common_11levenshtein_EditOperationType); /*proto*/
 static int __pyx_array_allocate_buffer(struct __pyx_array_obj *); /*proto*/
 static struct __pyx_array_obj *__pyx_array_new(PyObject *, Py_ssize_t, char *, char *, char *); /*proto*/
 static PyObject *__pyx_memoryview_new(PyObject *, int, int, __Pyx_TypeInfo *); /*proto*/
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *); /*proto*/
 static PyObject *_unellipsify(PyObject *, int); /*proto*/
 static int assert_direct_dimensions(Py_ssize_t *, int); /*proto*/
 static struct __pyx_memoryview_obj *__pyx_memview_slice(struct __pyx_memoryview_obj *, PyObject *); /*proto*/
@@ -3319,17 +3338,17 @@
 static const char __pyx_k_all_paths_with_heuristic[] = "all_paths_with_heuristic";
 static const char __pyx_k_Dimension_d_is_not_direct[] = "Dimension %d is not direct";
 static const char __pyx_k_Index_out_of_bounds_axis_d[] = "Index out of bounds (axis %d)";
 static const char __pyx_k_Step_may_not_be_zero_axis_d[] = "Step may not be zero (axis %d)";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_prolothar_common_levenshtein[] = "prolothar_common.levenshtein";
 static const char __pyx_k_pyx_unpickle_PathEnumeration[] = "__pyx_unpickle_PathEnumeration";
+static const char __pyx_k_Pyx_CFunc_3de20f__21prolothar[] = "__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e.<locals>.wrap";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_PathEnumeration__compute_lower[] = "_PathEnumeration__compute_lower_bound";
-static const char __pyx_k_Pyx_CFunc___lParenint__comma_i[] = "__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e.<locals>.wrap";
 static const char __pyx_k_This_file_is_part_of_Prolothar[] = "\n    This file is part of Prolothar-Rule-Mining (More Info: https://github.com/shs-it/prolothar-rule-mining).\n\n    Prolothar-Rule-Mining is free software: you can redistribute it and/or modify\n    it under the terms of the GNU General Public License as published by\n    the Free Software Foundation, either version 3 of the License, or\n    (at your option) any later version.\n\n    Prolothar-Rule-Mining is distributed in the hope that it will be useful,\n    but WITHOUT ANY WARRANTY; without even the implied warranty of\n    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the\n    GNU General Public License for more details.\n\n    You should have received a copy of the GNU General Public License\n    along with Prolothar-Rule-Mining. If not, see <https://www.gnu.org/licenses/>.\n";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_PathEnumeration___compute_lower[] = "PathEnumeration.__compute_lower_bound";
 static const char __pyx_k_PathEnumeration___reduce_cython[] = "PathEnumeration.__reduce_cython__";
 static const char __pyx_k_PathEnumeration__create_alignme[] = "_PathEnumeration__create_alignment";
 static const char __pyx_k_compute_alignment_locals_lambda[] = "compute_alignment.<locals>.<lambda>";
 static const char __pyx_k_All_dimensions_preceding_dimensi[] = "All dimensions preceding dimension %d must be indexed and not sliced";
@@ -3353,15 +3372,15 @@
 static const char __pyx_k_prolothar_rule_mining_models_eve[] = "prolothar_rule_mining.models.event_flow_graph.alignment.path_enumeration";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_2[] = "Incompatible checksums (0x%x vs (0xa9632b8, 0x8c6b243, 0x4d2146d) = (all_paths, graph))";
 static const char __pyx_k_prolothar_rule_mining_models_eve_2[] = "prolothar_rule_mining.models.event_flow_graph";
 static const char __pyx_k_prolothar_rule_mining_models_eve_3[] = "prolothar_rule_mining.models.event_flow_graph.alignment.alignment";
 static const char __pyx_k_prolothar_rule_mining_models_eve_4[] = "prolothar_rule_mining\\models\\event_flow_graph\\alignment\\path_enumeration.pyx";
 /* #### Code section: decls ### */
-static PyObject *__pyx_pf_11cfunc_dot_to_py_80__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_wrap(PyObject *__pyx_self, struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation *__pyx_v_e); /* proto */
+static PyObject *__pyx_pf_11cfunc_dot_to_py_80__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_wrap(PyObject *__pyx_self, struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation *__pyx_v_e); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -3404,15 +3423,15 @@
 static PyObject *__pyx_pf_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_15PathEnumeration_2compute_alignment(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration *__pyx_v_self, PyObject *__pyx_v_sequence); /* proto */
 static PyObject *__pyx_pf_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_15PathEnumeration_4__compute_lower_bound(CYTHON_UNUSED struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration *__pyx_v_self, PyObject *__pyx_v_path, PyObject *__pyx_v_sequence, PyObject *__pyx_v_events_in_sequence); /* proto */
 static PyObject *__pyx_pf_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_15PathEnumeration_6_PathEnumeration__create_alignment(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration *__pyx_v_self, PyObject *__pyx_v_best_path, PyObject *__pyx_v_sequence, __Pyx_memviewslice __pyx_v_best_cost_matrix); /* proto */
 static PyObject *__pyx_pf_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_15PathEnumeration_8__reduce_cython__(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_15PathEnumeration_10__setstate_cython__(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration___pyx_unpickle_PathEnumeration(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyList_Type_pop = {0, 0, 0, 0, 0};
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
@@ -3454,22 +3473,22 @@
   PyTypeObject *__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move;
   PyTypeObject *__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment;
   #if CYTHON_USE_MODULE_STATE
   #endif
   PyTypeObject *__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder;
   #if CYTHON_USE_MODULE_STATE
   PyObject *__pyx_type_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration;
-  PyObject *__pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e;
+  PyObject *__pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e;
   PyObject *__pyx_type___pyx_array;
   PyObject *__pyx_type___pyx_MemviewEnum;
   PyObject *__pyx_type___pyx_memoryview;
   PyObject *__pyx_type___pyx_memoryviewslice;
   #endif
   PyTypeObject *__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration;
-  PyTypeObject *__pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e;
+  PyTypeObject *__pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e;
   PyTypeObject *__pyx_array_type;
   PyTypeObject *__pyx_MemviewEnum_type;
   PyTypeObject *__pyx_memoryview_type;
   PyTypeObject *__pyx_memoryviewslice_type;
   PyObject *__pyx_n_s_ASCII;
   PyObject *__pyx_n_s_Alignment;
   PyObject *__pyx_kp_s_All_dimensions_preceding_dimensi;
@@ -3508,15 +3527,15 @@
   PyObject *__pyx_n_s_PathEnumeration___compute_lower;
   PyObject *__pyx_n_s_PathEnumeration___reduce_cython;
   PyObject *__pyx_n_s_PathEnumeration___setstate_cytho;
   PyObject *__pyx_n_s_PathEnumeration__compute_lower;
   PyObject *__pyx_n_s_PathEnumeration__create_alignme;
   PyObject *__pyx_n_s_PathEnumeration_compute_alignmen;
   PyObject *__pyx_n_s_PickleError;
-  PyObject *__pyx_n_s_Pyx_CFunc___lParenint__comma_i;
+  PyObject *__pyx_n_s_Pyx_CFunc_3de20f__21prolothar;
   PyObject *__pyx_n_s_SUBSTITUTE;
   PyObject *__pyx_n_s_Sequence;
   PyObject *__pyx_kp_s_Step_may_not_be_zero_axis_d;
   PyObject *__pyx_n_s_StopIteration;
   PyObject *__pyx_kp_s_Tuple_str;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
@@ -3750,16 +3769,16 @@
   Py_CLEAR(clear_module_state->__pyx_ptype_16prolothar_common_11levenshtein_EditOperation);
   Py_CLEAR(clear_module_state->__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node);
   Py_CLEAR(clear_module_state->__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move);
   Py_CLEAR(clear_module_state->__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment);
   Py_CLEAR(clear_module_state->__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder);
   Py_CLEAR(clear_module_state->__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration);
   Py_CLEAR(clear_module_state->__pyx_type_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration);
-  Py_CLEAR(clear_module_state->__pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e);
-  Py_CLEAR(clear_module_state->__pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e);
+  Py_CLEAR(clear_module_state->__pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e);
+  Py_CLEAR(clear_module_state->__pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e);
   Py_CLEAR(clear_module_state->__pyx_array_type);
   Py_CLEAR(clear_module_state->__pyx_type___pyx_array);
   Py_CLEAR(clear_module_state->__pyx_MemviewEnum_type);
   Py_CLEAR(clear_module_state->__pyx_type___pyx_MemviewEnum);
   Py_CLEAR(clear_module_state->__pyx_memoryview_type);
   Py_CLEAR(clear_module_state->__pyx_type___pyx_memoryview);
   Py_CLEAR(clear_module_state->__pyx_memoryviewslice_type);
@@ -3802,15 +3821,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_PathEnumeration___compute_lower);
   Py_CLEAR(clear_module_state->__pyx_n_s_PathEnumeration___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_PathEnumeration___setstate_cytho);
   Py_CLEAR(clear_module_state->__pyx_n_s_PathEnumeration__compute_lower);
   Py_CLEAR(clear_module_state->__pyx_n_s_PathEnumeration__create_alignme);
   Py_CLEAR(clear_module_state->__pyx_n_s_PathEnumeration_compute_alignmen);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
-  Py_CLEAR(clear_module_state->__pyx_n_s_Pyx_CFunc___lParenint__comma_i);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Pyx_CFunc_3de20f__21prolothar);
   Py_CLEAR(clear_module_state->__pyx_n_s_SUBSTITUTE);
   Py_CLEAR(clear_module_state->__pyx_n_s_Sequence);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Step_may_not_be_zero_axis_d);
   Py_CLEAR(clear_module_state->__pyx_n_s_StopIteration);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Tuple_str);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Unable_to_convert_item_to_object);
@@ -4022,16 +4041,16 @@
   Py_VISIT(traverse_module_state->__pyx_ptype_16prolothar_common_11levenshtein_EditOperation);
   Py_VISIT(traverse_module_state->__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node);
   Py_VISIT(traverse_module_state->__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move);
   Py_VISIT(traverse_module_state->__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment);
   Py_VISIT(traverse_module_state->__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder);
   Py_VISIT(traverse_module_state->__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration);
   Py_VISIT(traverse_module_state->__pyx_type_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration);
-  Py_VISIT(traverse_module_state->__pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e);
-  Py_VISIT(traverse_module_state->__pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e);
+  Py_VISIT(traverse_module_state->__pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e);
+  Py_VISIT(traverse_module_state->__pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e);
   Py_VISIT(traverse_module_state->__pyx_array_type);
   Py_VISIT(traverse_module_state->__pyx_type___pyx_array);
   Py_VISIT(traverse_module_state->__pyx_MemviewEnum_type);
   Py_VISIT(traverse_module_state->__pyx_type___pyx_MemviewEnum);
   Py_VISIT(traverse_module_state->__pyx_memoryview_type);
   Py_VISIT(traverse_module_state->__pyx_type___pyx_memoryview);
   Py_VISIT(traverse_module_state->__pyx_memoryviewslice_type);
@@ -4074,15 +4093,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_PathEnumeration___compute_lower);
   Py_VISIT(traverse_module_state->__pyx_n_s_PathEnumeration___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_PathEnumeration___setstate_cytho);
   Py_VISIT(traverse_module_state->__pyx_n_s_PathEnumeration__compute_lower);
   Py_VISIT(traverse_module_state->__pyx_n_s_PathEnumeration__create_alignme);
   Py_VISIT(traverse_module_state->__pyx_n_s_PathEnumeration_compute_alignmen);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
-  Py_VISIT(traverse_module_state->__pyx_n_s_Pyx_CFunc___lParenint__comma_i);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Pyx_CFunc_3de20f__21prolothar);
   Py_VISIT(traverse_module_state->__pyx_n_s_SUBSTITUTE);
   Py_VISIT(traverse_module_state->__pyx_n_s_Sequence);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Step_may_not_be_zero_axis_d);
   Py_VISIT(traverse_module_state->__pyx_n_s_StopIteration);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Tuple_str);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Unable_to_convert_item_to_object);
@@ -4312,22 +4331,22 @@
 #define __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move __pyx_mstate_global->__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move
 #define __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment __pyx_mstate_global->__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment
 #if CYTHON_USE_MODULE_STATE
 #endif
 #define __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder __pyx_mstate_global->__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder
 #if CYTHON_USE_MODULE_STATE
 #define __pyx_type_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration __pyx_mstate_global->__pyx_type_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration
-#define __pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e __pyx_mstate_global->__pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e
+#define __pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e __pyx_mstate_global->__pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e
 #define __pyx_type___pyx_array __pyx_mstate_global->__pyx_type___pyx_array
 #define __pyx_type___pyx_MemviewEnum __pyx_mstate_global->__pyx_type___pyx_MemviewEnum
 #define __pyx_type___pyx_memoryview __pyx_mstate_global->__pyx_type___pyx_memoryview
 #define __pyx_type___pyx_memoryviewslice __pyx_mstate_global->__pyx_type___pyx_memoryviewslice
 #endif
 #define __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration __pyx_mstate_global->__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration
-#define __pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e __pyx_mstate_global->__pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e
+#define __pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e __pyx_mstate_global->__pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e
 #define __pyx_array_type __pyx_mstate_global->__pyx_array_type
 #define __pyx_MemviewEnum_type __pyx_mstate_global->__pyx_MemviewEnum_type
 #define __pyx_memoryview_type __pyx_mstate_global->__pyx_memoryview_type
 #define __pyx_memoryviewslice_type __pyx_mstate_global->__pyx_memoryviewslice_type
 #define __pyx_n_s_ASCII __pyx_mstate_global->__pyx_n_s_ASCII
 #define __pyx_n_s_Alignment __pyx_mstate_global->__pyx_n_s_Alignment
 #define __pyx_kp_s_All_dimensions_preceding_dimensi __pyx_mstate_global->__pyx_kp_s_All_dimensions_preceding_dimensi
@@ -4366,15 +4385,15 @@
 #define __pyx_n_s_PathEnumeration___compute_lower __pyx_mstate_global->__pyx_n_s_PathEnumeration___compute_lower
 #define __pyx_n_s_PathEnumeration___reduce_cython __pyx_mstate_global->__pyx_n_s_PathEnumeration___reduce_cython
 #define __pyx_n_s_PathEnumeration___setstate_cytho __pyx_mstate_global->__pyx_n_s_PathEnumeration___setstate_cytho
 #define __pyx_n_s_PathEnumeration__compute_lower __pyx_mstate_global->__pyx_n_s_PathEnumeration__compute_lower
 #define __pyx_n_s_PathEnumeration__create_alignme __pyx_mstate_global->__pyx_n_s_PathEnumeration__create_alignme
 #define __pyx_n_s_PathEnumeration_compute_alignmen __pyx_mstate_global->__pyx_n_s_PathEnumeration_compute_alignmen
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
-#define __pyx_n_s_Pyx_CFunc___lParenint__comma_i __pyx_mstate_global->__pyx_n_s_Pyx_CFunc___lParenint__comma_i
+#define __pyx_n_s_Pyx_CFunc_3de20f__21prolothar __pyx_mstate_global->__pyx_n_s_Pyx_CFunc_3de20f__21prolothar
 #define __pyx_n_s_SUBSTITUTE __pyx_mstate_global->__pyx_n_s_SUBSTITUTE
 #define __pyx_n_s_Sequence __pyx_mstate_global->__pyx_n_s_Sequence
 #define __pyx_kp_s_Step_may_not_be_zero_axis_d __pyx_mstate_global->__pyx_kp_s_Step_may_not_be_zero_axis_d
 #define __pyx_n_s_StopIteration __pyx_mstate_global->__pyx_n_s_StopIteration
 #define __pyx_kp_s_Tuple_str __pyx_mstate_global->__pyx_kp_s_Tuple_str
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_kp_s_Unable_to_convert_item_to_object __pyx_mstate_global->__pyx_kp_s_Unable_to_convert_item_to_object
@@ -4562,32 +4581,32 @@
 #define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
 #define __pyx_codeobj__31 __pyx_mstate_global->__pyx_codeobj__31
 #define __pyx_codeobj__33 __pyx_mstate_global->__pyx_codeobj__33
 #define __pyx_codeobj__34 __pyx_mstate_global->__pyx_codeobj__34
 /* #### Code section: module_code ### */
 
 /* "cfunc.to_py":67
- * @cname("__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e")
- * cdef object __Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e((int, int)  (*f)(EditOperation) except *):
+ * @cname("__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e")
+ * cdef object __Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e((int, int)  (*f)(EditOperation) except *):
  *     def wrap(EditOperation e):             # <<<<<<<<<<<<<<
  *         """wrap(e: 'EditOperation') -> '(int, int) '"""
  *         return f(e)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_11cfunc_dot_to_py_80__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_1wrap(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_11cfunc_dot_to_py_80__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_1wrap(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_11cfunc_dot_to_py_80__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_wrap, "wrap(e: 'EditOperation') -> '(int, int) '");
-static PyMethodDef __pyx_mdef_11cfunc_dot_to_py_80__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_1wrap = {"wrap", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_11cfunc_dot_to_py_80__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_1wrap, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_11cfunc_dot_to_py_80__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_wrap};
-static PyObject *__pyx_pw_11cfunc_dot_to_py_80__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_1wrap(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_11cfunc_dot_to_py_80__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_wrap, "wrap(e: 'EditOperation') -> '(int, int) '");
+static PyMethodDef __pyx_mdef_11cfunc_dot_to_py_80__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_1wrap = {"wrap", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_11cfunc_dot_to_py_80__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_1wrap, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_11cfunc_dot_to_py_80__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_wrap};
+static PyObject *__pyx_pw_11cfunc_dot_to_py_80__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_1wrap(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation *__pyx_v_e = 0;
@@ -4649,20 +4668,20 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("cfunc.to_py.__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e.wrap", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("cfunc.to_py.__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e.wrap", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_e), __pyx_ptype_16prolothar_common_11levenshtein_EditOperation, 1, "e", 0))) __PYX_ERR(1, 67, __pyx_L1_error)
-  __pyx_r = __pyx_pf_11cfunc_dot_to_py_80__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_wrap(__pyx_self, __pyx_v_e);
+  __pyx_r = __pyx_pf_11cfunc_dot_to_py_80__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_wrap(__pyx_self, __pyx_v_e);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -4671,26 +4690,26 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_11cfunc_dot_to_py_80__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_wrap(PyObject *__pyx_self, struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation *__pyx_v_e) {
-  struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e *__pyx_cur_scope;
-  struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e *__pyx_outer_scope;
+static PyObject *__pyx_pf_11cfunc_dot_to_py_80__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_wrap(PyObject *__pyx_self, struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation *__pyx_v_e) {
+  struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e *__pyx_cur_scope;
+  struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e *__pyx_outer_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __pyx_ctuple_int__and_int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wrap", 1);
-  __pyx_outer_scope = (struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e *) __Pyx_CyFunction_GetClosure(__pyx_self);
+  __pyx_outer_scope = (struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
 
   /* "cfunc.to_py":69
  *     def wrap(EditOperation e):
  *         """wrap(e: 'EditOperation') -> '(int, int) '"""
  *         return f(e)             # <<<<<<<<<<<<<<
  *     return wrap
@@ -4701,68 +4720,68 @@
   __pyx_t_2 = __pyx_convert__to_py___pyx_ctuple_int__and_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "cfunc.to_py":67
- * @cname("__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e")
- * cdef object __Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e((int, int)  (*f)(EditOperation) except *):
+ * @cname("__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e")
+ * cdef object __Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e((int, int)  (*f)(EditOperation) except *):
  *     def wrap(EditOperation e):             # <<<<<<<<<<<<<<
  *         """wrap(e: 'EditOperation') -> '(int, int) '"""
  *         return f(e)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("cfunc.to_py.__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e.wrap", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("cfunc.to_py.__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e.wrap", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cfunc.to_py":66
  * 
- * @cname("__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e")
- * cdef object __Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e((int, int)  (*f)(EditOperation) except *):             # <<<<<<<<<<<<<<
+ * @cname("__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e")
+ * cdef object __Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e((int, int)  (*f)(EditOperation) except *):             # <<<<<<<<<<<<<<
  *     def wrap(EditOperation e):
  *         """wrap(e: 'EditOperation') -> '(int, int) '"""
  */
 
-static PyObject *__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e(__pyx_ctuple_int__and_int (*__pyx_v_f)(struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation *)) {
-  struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e *__pyx_cur_scope;
+static PyObject *__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e(__pyx_ctuple_int__and_int (*__pyx_v_f)(struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation *)) {
+  struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e *__pyx_cur_scope;
   PyObject *__pyx_v_wrap = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e", 0);
-  __pyx_cur_scope = (struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e *)__pyx_tp_new___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e(__pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e, __pyx_empty_tuple, NULL);
+  __Pyx_RefNannySetupContext("__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e", 0);
+  __pyx_cur_scope = (struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e *)__pyx_tp_new___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e(__pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(1, 66, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_f = __pyx_v_f;
 
   /* "cfunc.to_py":67
- * @cname("__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e")
- * cdef object __Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e((int, int)  (*f)(EditOperation) except *):
+ * @cname("__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e")
+ * cdef object __Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e((int, int)  (*f)(EditOperation) except *):
  *     def wrap(EditOperation e):             # <<<<<<<<<<<<<<
  *         """wrap(e: 'EditOperation') -> '(int, int) '"""
  *         return f(e)
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11cfunc_dot_to_py_80__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_1wrap, 0, __pyx_n_s_Pyx_CFunc___lParenint__comma_i, ((PyObject*)__pyx_cur_scope), __pyx_n_s_cfunc_to_py, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 67, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11cfunc_dot_to_py_80__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_1wrap, 0, __pyx_n_s_Pyx_CFunc_3de20f__21prolothar, ((PyObject*)__pyx_cur_scope), __pyx_n_s_cfunc_to_py, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_wrap = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "cfunc.to_py":70
  *         """wrap(e: 'EditOperation') -> '(int, int) '"""
  *         return f(e)
@@ -4773,364 +4792,427 @@
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_wrap);
   __pyx_r = __pyx_v_wrap;
   goto __pyx_L0;
 
   /* "cfunc.to_py":66
  * 
- * @cname("__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e")
- * cdef object __Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e((int, int)  (*f)(EditOperation) except *):             # <<<<<<<<<<<<<<
+ * @cname("__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e")
+ * cdef object __Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e((int, int)  (*f)(EditOperation) except *):             # <<<<<<<<<<<<<<
  *     def wrap(EditOperation e):
  *         """wrap(e: 'EditOperation') -> '(int, int) '"""
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("cfunc.to_py.__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("cfunc.to_py.__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_wrap);
   __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "EnumTypeToPy":132
+/* "EnumTypeToPy":4
  * 
- * @cname("__Pyx_Enum_bca7cc__enum__dunderpyx_t_16prolothar_common_11levenshtein_EditOperationType__etc_to_py")
- * cdef __Pyx_Enum_bca7cc__enum__dunderpyx_t_16prolothar_common_11levenshtein_EditOperationType__etc_to_py(EditOperationType c_val):             # <<<<<<<<<<<<<<
+ * @cname("__Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py")
+ * cdef __Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py(EditOperationType c_val):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_enum
- * 
+ *     global __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py
  */
 
-static PyObject *__Pyx_Enum_bca7cc__enum__dunderpyx_t_16prolothar_common_11levenshtein_EditOperationType__etc_to_py(enum __pyx_t_16prolothar_common_11levenshtein_EditOperationType __pyx_v_c_val) {
+static PyObject *__Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py(enum __pyx_t_16prolothar_common_11levenshtein_EditOperationType __pyx_v_c_val) {
   PyObject *__pyx_v___pyx_enum = 0;
   PyObject *__pyx_v_warnings = NULL;
   int __pyx_v_underlying_c_val;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__Pyx_Enum_bca7cc__enum__dunderpyx_t_16prolothar_common_11levenshtein_EditOperationType__etc_to_py", 1);
+  __Pyx_RefNannySetupContext("__Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py", 1);
 
-  /* "EnumTypeToPy":137
+  /* "EnumTypeToPy":11
  * 
  * 
- *     try:             # <<<<<<<<<<<<<<
- *         from prolothar_common.levenshtein import EditOperationType as __pyx_enum
- *     except ImportError:
+ *     if __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py is None:             # <<<<<<<<<<<<<<
+ *         try:
+ *             from prolothar_common.levenshtein import EditOperationType as __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py
  */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
+  __pyx_t_1 = (__pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py == Py_None);
+  if (__pyx_t_1) {
 
-      /* "EnumTypeToPy":138
+    /* "EnumTypeToPy":12
  * 
- *     try:
- *         from prolothar_common.levenshtein import EditOperationType as __pyx_enum             # <<<<<<<<<<<<<<
- *     except ImportError:
- *         import warnings
+ *     if __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py is None:
+ *         try:             # <<<<<<<<<<<<<<
+ *             from prolothar_common.levenshtein import EditOperationType as __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py
+ *         except ImportError:
  */
-      __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 138, __pyx_L3_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_INCREF(__pyx_n_s_EditOperationType);
-      __Pyx_GIVEREF(__pyx_n_s_EditOperationType);
-      if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_n_s_EditOperationType)) __PYX_ERR(1, 138, __pyx_L3_error);
-      __pyx_t_5 = __Pyx_Import(__pyx_n_s_prolothar_common_levenshtein, __pyx_t_4, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 138, __pyx_L3_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_ImportFrom(__pyx_t_5, __pyx_n_s_EditOperationType); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 138, __pyx_L3_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_4);
-      __pyx_v___pyx_enum = __pyx_t_4;
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    {
+      __Pyx_PyThreadState_declare
+      __Pyx_PyThreadState_assign
+      __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
+      __Pyx_XGOTREF(__pyx_t_2);
+      __Pyx_XGOTREF(__pyx_t_3);
+      __Pyx_XGOTREF(__pyx_t_4);
+      /*try:*/ {
 
-      /* "EnumTypeToPy":137
- * 
- * 
- *     try:             # <<<<<<<<<<<<<<
- *         from prolothar_common.levenshtein import EditOperationType as __pyx_enum
- *     except ImportError:
+        /* "EnumTypeToPy":13
+ *     if __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py is None:
+ *         try:
+ *             from prolothar_common.levenshtein import EditOperationType as __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py             # <<<<<<<<<<<<<<
+ *         except ImportError:
+ *             __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py = False  # False indicates "don't try again"
  */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L4_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __Pyx_INCREF(__pyx_n_s_EditOperationType);
+        __Pyx_GIVEREF(__pyx_n_s_EditOperationType);
+        if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_EditOperationType)) __PYX_ERR(1, 13, __pyx_L4_error);
+        __pyx_t_6 = __Pyx_Import(__pyx_n_s_prolothar_common_levenshtein, __pyx_t_5, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 13, __pyx_L4_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __pyx_t_5 = __Pyx_ImportFrom(__pyx_t_6, __pyx_n_s_EditOperationType); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L4_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_XGOTREF(__pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py);
+        __Pyx_DECREF_SET(__pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py, __pyx_t_5);
+        __Pyx_GIVEREF(__pyx_t_5);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "EnumTypeToPy":139
- *     try:
- *         from prolothar_common.levenshtein import EditOperationType as __pyx_enum
- *     except ImportError:             # <<<<<<<<<<<<<<
- *         import warnings
- *         warnings.warn(
+        /* "EnumTypeToPy":12
+ * 
+ *     if __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py is None:
+ *         try:             # <<<<<<<<<<<<<<
+ *             from prolothar_common.levenshtein import EditOperationType as __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py
+ *         except ImportError:
  */
-    __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ImportError);
-    if (__pyx_t_6) {
-      __Pyx_AddTraceback("EnumTypeToPy.__Pyx_Enum_bca7cc__enum__dunderpyx_t_16prolothar_common_11levenshtein_EditOperationType__etc_to_py", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(1, 139, __pyx_L5_except_error)
-      __Pyx_XGOTREF(__pyx_t_5);
-      __Pyx_XGOTREF(__pyx_t_4);
-      __Pyx_XGOTREF(__pyx_t_7);
+      }
+      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      goto __pyx_L9_try_end;
+      __pyx_L4_error:;
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "EnumTypeToPy":140
- *         from prolothar_common.levenshtein import EditOperationType as __pyx_enum
- *     except ImportError:
- *         import warnings             # <<<<<<<<<<<<<<
- *         warnings.warn(
- *             f"enum class EditOperationType not importable from prolothar_common.levenshtein. "
- */
-      __pyx_t_8 = __Pyx_ImportDottedModule(__pyx_n_s_warnings, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 140, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __pyx_v_warnings = __pyx_t_8;
-      __pyx_t_8 = 0;
+      /* "EnumTypeToPy":14
+ *         try:
+ *             from prolothar_common.levenshtein import EditOperationType as __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py
+ *         except ImportError:             # <<<<<<<<<<<<<<
+ *             __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py = False  # False indicates "don't try again"
+ *             import warnings
+ */
+      __pyx_t_7 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ImportError);
+      if (__pyx_t_7) {
+        __Pyx_AddTraceback("EnumTypeToPy.__Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py", __pyx_clineno, __pyx_lineno, __pyx_filename);
+        if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_5, &__pyx_t_8) < 0) __PYX_ERR(1, 14, __pyx_L6_except_error)
+        __Pyx_XGOTREF(__pyx_t_6);
+        __Pyx_XGOTREF(__pyx_t_5);
+        __Pyx_XGOTREF(__pyx_t_8);
 
-      /* "EnumTypeToPy":141
- *     except ImportError:
- *         import warnings
- *         warnings.warn(             # <<<<<<<<<<<<<<
- *             f"enum class EditOperationType not importable from prolothar_common.levenshtein. "
- *             "You are probably using a cpdef enum declared in a .pxd file that "
- */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_warnings, __pyx_n_s_warn); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 141, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_10 = NULL;
-      __pyx_t_6 = 0;
-      #if CYTHON_UNPACK_METHODS
-      if (likely(PyMethod_Check(__pyx_t_9))) {
-        __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
-        if (likely(__pyx_t_10)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-          __Pyx_INCREF(__pyx_t_10);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_9, function);
-          __pyx_t_6 = 1;
+        /* "EnumTypeToPy":15
+ *             from prolothar_common.levenshtein import EditOperationType as __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py
+ *         except ImportError:
+ *             __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py = False  # False indicates "don't try again"             # <<<<<<<<<<<<<<
+ *             import warnings
+ *             warnings.warn(
+ */
+        __Pyx_INCREF(Py_False);
+        __Pyx_XGOTREF(__pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py);
+        __Pyx_DECREF_SET(__pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py, Py_False);
+        __Pyx_GIVEREF(Py_False);
+
+        /* "EnumTypeToPy":16
+ *         except ImportError:
+ *             __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py = False  # False indicates "don't try again"
+ *             import warnings             # <<<<<<<<<<<<<<
+ *             warnings.warn(
+ *                 f"enum class EditOperationType not importable from prolothar_common.levenshtein. "
+ */
+        __pyx_t_9 = __Pyx_ImportDottedModule(__pyx_n_s_warnings, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 16, __pyx_L6_except_error)
+        __Pyx_GOTREF(__pyx_t_9);
+        __pyx_v_warnings = __pyx_t_9;
+        __pyx_t_9 = 0;
+
+        /* "EnumTypeToPy":17
+ *             __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py = False  # False indicates "don't try again"
+ *             import warnings
+ *             warnings.warn(             # <<<<<<<<<<<<<<
+ *                 f"enum class EditOperationType not importable from prolothar_common.levenshtein. "
+ *                 "You are probably using a cpdef enum declared in a .pxd file that "
+ */
+        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_warnings, __pyx_n_s_warn); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 17, __pyx_L6_except_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __pyx_t_11 = NULL;
+        __pyx_t_7 = 0;
+        #if CYTHON_UNPACK_METHODS
+        if (likely(PyMethod_Check(__pyx_t_10))) {
+          __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_10);
+          if (likely(__pyx_t_11)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+            __Pyx_INCREF(__pyx_t_11);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_10, function);
+            __pyx_t_7 = 1;
+          }
+        }
+        #endif
+        {
+          PyObject *__pyx_callargs[2] = {__pyx_t_11, __pyx_kp_u_enum_class_EditOperationType_not};
+          __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+          __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 17, __pyx_L6_except_error)
+          __Pyx_GOTREF(__pyx_t_9);
+          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         }
-      }
-      #endif
-      {
-        PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_kp_u_enum_class_EditOperationType_not};
-        __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
-        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-        if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 141, __pyx_L5_except_error)
-        __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+        goto __pyx_L5_exception_handled;
       }
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      goto __pyx_L6_except_error;
 
-      /* "EnumTypeToPy":145
- *             "You are probably using a cpdef enum declared in a .pxd file that "
- *             "does not have a .py  or .pyx file.")
- *         return <int>c_val             # <<<<<<<<<<<<<<
+      /* "EnumTypeToPy":12
  * 
- *     if 0:
+ *     if __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py is None:
+ *         try:             # <<<<<<<<<<<<<<
+ *             from prolothar_common.levenshtein import EditOperationType as __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py
+ *         except ImportError:
  */
-      __Pyx_XDECREF(__pyx_r);
-      __pyx_t_8 = __Pyx_PyInt_From_int(((int)__pyx_v_c_val)); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 145, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __pyx_r = __pyx_t_8;
-      __pyx_t_8 = 0;
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      goto __pyx_L6_except_return;
+      __pyx_L6_except_error:;
+      __Pyx_XGIVEREF(__pyx_t_2);
+      __Pyx_XGIVEREF(__pyx_t_3);
+      __Pyx_XGIVEREF(__pyx_t_4);
+      __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
+      goto __pyx_L1_error;
+      __pyx_L5_exception_handled:;
+      __Pyx_XGIVEREF(__pyx_t_2);
+      __Pyx_XGIVEREF(__pyx_t_3);
+      __Pyx_XGIVEREF(__pyx_t_4);
+      __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
+      __pyx_L9_try_end:;
     }
-    goto __pyx_L5_except_error;
 
-    /* "EnumTypeToPy":137
+    /* "EnumTypeToPy":11
  * 
  * 
- *     try:             # <<<<<<<<<<<<<<
- *         from prolothar_common.levenshtein import EditOperationType as __pyx_enum
- *     except ImportError:
+ *     if __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py is None:             # <<<<<<<<<<<<<<
+ *         try:
+ *             from prolothar_common.levenshtein import EditOperationType as __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py
  */
-    __pyx_L5_except_error:;
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L6_except_return:;
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+  }
+
+  /* "EnumTypeToPy":21
+ *                 "You are probably using a cpdef enum declared in a .pxd file that "
+ *                 "does not have a .py  or .pyx file.")
+ *     if __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py is False:             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_t_1 = (__pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py == Py_False);
+  if (__pyx_t_1) {
+
+    /* "EnumTypeToPy":24
+ * 
+ * 
+ *         return <int>c_val             # <<<<<<<<<<<<<<
+ *     __pyx_enum = __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py
+ * 
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_8 = __Pyx_PyInt_From_int(((int)__pyx_v_c_val)); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 24, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_r = __pyx_t_8;
+    __pyx_t_8 = 0;
     goto __pyx_L0;
-    __pyx_L8_try_end:;
+
+    /* "EnumTypeToPy":21
+ *                 "You are probably using a cpdef enum declared in a .pxd file that "
+ *                 "does not have a .py  or .pyx file.")
+ *     if __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py is False:             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
   }
 
-  /* "EnumTypeToPy":147
+  /* "EnumTypeToPy":25
+ * 
  *         return <int>c_val
+ *     __pyx_enum = __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py             # <<<<<<<<<<<<<<
+ * 
+ *     if 0:
+ */
+  __Pyx_INCREF(__pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py);
+  __pyx_v___pyx_enum = __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py;
+
+  /* "EnumTypeToPy":27
+ *     __pyx_enum = __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py
  * 
  *     if 0:             # <<<<<<<<<<<<<<
  *         pass
  *     elif c_val == EditOperationType.DELETE:
  */
   switch (__pyx_v_c_val) {
     case __pyx_e_16prolothar_common_11levenshtein_DELETE:
 
-    /* "EnumTypeToPy":150
+    /* "EnumTypeToPy":30
  *         pass
  *     elif c_val == EditOperationType.DELETE:
  *         return __pyx_enum.DELETE             # <<<<<<<<<<<<<<
  *     elif c_val == EditOperationType.INSERT:
  *         return __pyx_enum.INSERT
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_DELETE); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 150, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_r = __pyx_t_7;
-    __pyx_t_7 = 0;
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_DELETE); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 30, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_r = __pyx_t_8;
+    __pyx_t_8 = 0;
     goto __pyx_L0;
 
-    /* "EnumTypeToPy":149
+    /* "EnumTypeToPy":29
  *     if 0:
  *         pass
  *     elif c_val == EditOperationType.DELETE:             # <<<<<<<<<<<<<<
  *         return __pyx_enum.DELETE
  *     elif c_val == EditOperationType.INSERT:
  */
     break;
     case __pyx_e_16prolothar_common_11levenshtein_INSERT:
 
-    /* "EnumTypeToPy":152
+    /* "EnumTypeToPy":32
  *         return __pyx_enum.DELETE
  *     elif c_val == EditOperationType.INSERT:
  *         return __pyx_enum.INSERT             # <<<<<<<<<<<<<<
  *     elif c_val == EditOperationType.SUBSTITUTE:
  *         return __pyx_enum.SUBSTITUTE
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_INSERT); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 152, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_r = __pyx_t_7;
-    __pyx_t_7 = 0;
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_INSERT); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 32, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_r = __pyx_t_8;
+    __pyx_t_8 = 0;
     goto __pyx_L0;
 
-    /* "EnumTypeToPy":151
+    /* "EnumTypeToPy":31
  *     elif c_val == EditOperationType.DELETE:
  *         return __pyx_enum.DELETE
  *     elif c_val == EditOperationType.INSERT:             # <<<<<<<<<<<<<<
  *         return __pyx_enum.INSERT
  *     elif c_val == EditOperationType.SUBSTITUTE:
  */
     break;
     case __pyx_e_16prolothar_common_11levenshtein_SUBSTITUTE:
 
-    /* "EnumTypeToPy":154
+    /* "EnumTypeToPy":34
  *         return __pyx_enum.INSERT
  *     elif c_val == EditOperationType.SUBSTITUTE:
  *         return __pyx_enum.SUBSTITUTE             # <<<<<<<<<<<<<<
  *     else:
  *         underlying_c_val = <int>c_val
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_SUBSTITUTE); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 154, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_r = __pyx_t_7;
-    __pyx_t_7 = 0;
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_SUBSTITUTE); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 34, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_r = __pyx_t_8;
+    __pyx_t_8 = 0;
     goto __pyx_L0;
 
-    /* "EnumTypeToPy":153
+    /* "EnumTypeToPy":33
  *     elif c_val == EditOperationType.INSERT:
  *         return __pyx_enum.INSERT
  *     elif c_val == EditOperationType.SUBSTITUTE:             # <<<<<<<<<<<<<<
  *         return __pyx_enum.SUBSTITUTE
  *     else:
  */
     break;
     default:
 
-    /* "EnumTypeToPy":156
+    /* "EnumTypeToPy":36
  *         return __pyx_enum.SUBSTITUTE
  *     else:
  *         underlying_c_val = <int>c_val             # <<<<<<<<<<<<<<
  *         return __pyx_enum(underlying_c_val)
  * 
  */
     __pyx_v_underlying_c_val = ((int)__pyx_v_c_val);
 
-    /* "EnumTypeToPy":157
+    /* "EnumTypeToPy":37
  *     else:
  *         underlying_c_val = <int>c_val
  *         return __pyx_enum(underlying_c_val)             # <<<<<<<<<<<<<<
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_underlying_c_val); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 157, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_underlying_c_val); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 37, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_v___pyx_enum);
-    __pyx_t_5 = __pyx_v___pyx_enum; __pyx_t_8 = NULL;
-    __pyx_t_6 = 0;
+    __pyx_t_6 = __pyx_v___pyx_enum; __pyx_t_9 = NULL;
+    __pyx_t_7 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_8)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_8);
+    if (unlikely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_9)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
-        __pyx_t_6 = 1;
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __pyx_t_7 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_t_4};
-      __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
-      __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 157, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
+      PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_5};
+      __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 37, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
-    __pyx_r = __pyx_t_7;
-    __pyx_t_7 = 0;
+    __pyx_r = __pyx_t_8;
+    __pyx_t_8 = 0;
     goto __pyx_L0;
     break;
   }
 
-  /* "EnumTypeToPy":132
+  /* "EnumTypeToPy":4
  * 
- * @cname("__Pyx_Enum_bca7cc__enum__dunderpyx_t_16prolothar_common_11levenshtein_EditOperationType__etc_to_py")
- * cdef __Pyx_Enum_bca7cc__enum__dunderpyx_t_16prolothar_common_11levenshtein_EditOperationType__etc_to_py(EditOperationType c_val):             # <<<<<<<<<<<<<<
+ * @cname("__Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py")
+ * cdef __Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py(EditOperationType c_val):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_enum
- * 
+ *     global __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_AddTraceback("EnumTypeToPy.__Pyx_Enum_bca7cc__enum__dunderpyx_t_16prolothar_common_11levenshtein_EditOperationType__etc_to_py", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_AddTraceback("EnumTypeToPy.__Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_enum);
   __Pyx_XDECREF(__pyx_v_warnings);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -20776,15 +20858,15 @@
  *                 backtrace(best_path, sequence, best_cost_matrix),
  *                 key=edit_operation_sort):             # <<<<<<<<<<<<<<
  *             for i in range(model_index, edit_operation.i):
  *                 alignment.append_sync_move(best_path[i], sequence_index)
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e(__pyx_f_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_edit_operation_sort); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e(__pyx_f_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_edit_operation_sort); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_key, __pyx_t_4) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "prolothar_rule_mining/models/event_flow_graph/alignment/path_enumeration.pyx":112
  *         cdef int model_index = 0
  *         cdef int sequence_index = 0
@@ -20999,15 +21081,15 @@
  *             sequence_index = edit_operation.j
  *             if edit_operation.operation_type == EditOperationType.DELETE:             # <<<<<<<<<<<<<<
  *                 alignment.append_model_move(best_path[edit_operation.i])
  *                 model_index += 1
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_edit_operation, __pyx_n_s_operation_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_Enum_bca7cc__enum__dunderpyx_t_16prolothar_common_11levenshtein_EditOperationType__etc_to_py(__pyx_e_16prolothar_common_11levenshtein_DELETE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py(__pyx_e_16prolothar_common_11levenshtein_DELETE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_11 < 0))) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (__pyx_t_11) {
@@ -21058,15 +21140,15 @@
  *                 model_index += 1
  *             elif edit_operation.operation_type == EditOperationType.INSERT:             # <<<<<<<<<<<<<<
  *                 alignment.append_log_move(edit_operation.j)
  *                 sequence_index += 1
  */
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_edit_operation, __pyx_n_s_operation_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_Enum_bca7cc__enum__dunderpyx_t_16prolothar_common_11levenshtein_EditOperationType__etc_to_py(__pyx_e_16prolothar_common_11levenshtein_INSERT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py(__pyx_e_16prolothar_common_11levenshtein_INSERT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_11 < 0))) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (__pyx_t_11) {
@@ -22393,15 +22475,19 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->all_paths);
-  PyObject_GC_Track(o);
+  #if PY_MAJOR_VERSION < 3
+  if (!(__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder) || PyType_IS_GC(__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder)) PyObject_GC_Track(o);
+  #else
+  if (PyType_IS_GC(__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder)) PyObject_GC_Track(o);
+  #endif
   if (likely(__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder)) __Pyx_PyType_GetSlot(__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder, tp_dealloc, destructor)(o); else __Pyx_call_next_tp_dealloc(o, __pyx_tp_dealloc_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration);
 }
 
 static int __pyx_tp_traverse_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration *p = (struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration *)o;
   e = ((likely(__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder)) ? ((__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder->tp_traverse) ? __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder->tp_traverse(o, v, a) : 0) : __Pyx_call_next_tp_traverse(o, v, a, __pyx_tp_traverse_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration)); if (e) return e;
@@ -22526,83 +22612,85 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
-static struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e *__pyx_freelist___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e[8];
-static int __pyx_freecount___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e = 0;
+#if CYTHON_USE_FREELISTS
+static struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e *__pyx_freelist___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e[8];
+static int __pyx_freecount___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e = 0;
+#endif
 
-static PyObject *__pyx_tp_new___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
-  if (likely((int)(__pyx_freecount___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e)))) {
-    o = (PyObject*)__pyx_freelist___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e[--__pyx_freecount___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e];
-    memset(o, 0, sizeof(struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e));
+  #if CYTHON_USE_FREELISTS
+  if (likely((int)(__pyx_freecount___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e)))) {
+    o = (PyObject*)__pyx_freelist___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e[--__pyx_freecount___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e];
+    memset(o, 0, sizeof(struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e));
     (void) PyObject_INIT(o, t);
   } else
   #endif
   {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   #endif
   return o;
 }
 
-static void __pyx_tp_dealloc___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e(PyObject *o) {
+static void __pyx_tp_dealloc___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
-    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
-  #if CYTHON_COMPILING_IN_CPYTHON
-  if (((int)(__pyx_freecount___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e)))) {
-    __pyx_freelist___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e[__pyx_freecount___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e++] = ((struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e *)o);
+  #if CYTHON_USE_FREELISTS
+  if (((int)(__pyx_freecount___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e)))) {
+    __pyx_freelist___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e[__pyx_freecount___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e++] = ((struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
     #else
     {
       freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
       if (tp_free) tp_free(o);
     }
     #endif
   }
 }
 #if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_slots[] = {
-  {Py_tp_dealloc, (void *)__pyx_tp_dealloc___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e},
-  {Py_tp_new, (void *)__pyx_tp_new___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e},
+static PyType_Slot __pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e},
+  {Py_tp_new, (void *)__pyx_tp_new___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e},
   {0, 0},
 };
-static PyType_Spec __pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_spec = {
-  "prolothar_rule_mining.models.event_flow_graph.alignment.path_enumeration.__pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e",
-  sizeof(struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e),
+static PyType_Spec __pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_spec = {
+  "prolothar_rule_mining.models.event_flow_graph.alignment.path_enumeration.__pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e",
+  sizeof(struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e),
   0,
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_FINALIZE,
-  __pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_slots,
+  __pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_slots,
 };
 #else
 
-static PyTypeObject __pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e = {
+static PyTypeObject __pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e = {
   PyVarObject_HEAD_INIT(0, 0)
-  "prolothar_rule_mining.models.event_flow_graph.alignment.path_enumeration.""__pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e", /*tp_name*/
-  sizeof(struct __pyx_obj___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e), /*tp_basicsize*/
+  "prolothar_rule_mining.models.event_flow_graph.alignment.path_enumeration.""__pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e", /*tp_name*/
+  sizeof(struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e, /*tp_dealloc*/
+  __pyx_tp_dealloc___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -22639,15 +22727,15 @@
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
   #endif
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e, /*tp_new*/
+  __pyx_tp_new___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -23677,15 +23765,15 @@
     {&__pyx_n_s_PathEnumeration___compute_lower, __pyx_k_PathEnumeration___compute_lower, sizeof(__pyx_k_PathEnumeration___compute_lower), 0, 0, 1, 1},
     {&__pyx_n_s_PathEnumeration___reduce_cython, __pyx_k_PathEnumeration___reduce_cython, sizeof(__pyx_k_PathEnumeration___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_PathEnumeration___setstate_cytho, __pyx_k_PathEnumeration___setstate_cytho, sizeof(__pyx_k_PathEnumeration___setstate_cytho), 0, 0, 1, 1},
     {&__pyx_n_s_PathEnumeration__compute_lower, __pyx_k_PathEnumeration__compute_lower, sizeof(__pyx_k_PathEnumeration__compute_lower), 0, 0, 1, 1},
     {&__pyx_n_s_PathEnumeration__create_alignme, __pyx_k_PathEnumeration__create_alignme, sizeof(__pyx_k_PathEnumeration__create_alignme), 0, 0, 1, 1},
     {&__pyx_n_s_PathEnumeration_compute_alignmen, __pyx_k_PathEnumeration_compute_alignmen, sizeof(__pyx_k_PathEnumeration_compute_alignmen), 0, 0, 1, 1},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
-    {&__pyx_n_s_Pyx_CFunc___lParenint__comma_i, __pyx_k_Pyx_CFunc___lParenint__comma_i, sizeof(__pyx_k_Pyx_CFunc___lParenint__comma_i), 0, 0, 1, 1},
+    {&__pyx_n_s_Pyx_CFunc_3de20f__21prolothar, __pyx_k_Pyx_CFunc_3de20f__21prolothar, sizeof(__pyx_k_Pyx_CFunc_3de20f__21prolothar), 0, 0, 1, 1},
     {&__pyx_n_s_SUBSTITUTE, __pyx_k_SUBSTITUTE, sizeof(__pyx_k_SUBSTITUTE), 0, 0, 1, 1},
     {&__pyx_n_s_Sequence, __pyx_k_Sequence, sizeof(__pyx_k_Sequence), 0, 0, 1, 1},
     {&__pyx_kp_s_Step_may_not_be_zero_axis_d, __pyx_k_Step_may_not_be_zero_axis_d, sizeof(__pyx_k_Step_may_not_be_zero_axis_d), 0, 0, 1, 0},
     {&__pyx_n_s_StopIteration, __pyx_k_StopIteration, sizeof(__pyx_k_StopIteration), 0, 0, 1, 1},
     {&__pyx_kp_s_Tuple_str, __pyx_k_Tuple_str, sizeof(__pyx_k_Tuple_str), 0, 0, 1, 0},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
@@ -23841,15 +23929,15 @@
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 46, __pyx_L1_error)
   __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 60, __pyx_L1_error)
   __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 112, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 115, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 139, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 14, __pyx_L1_error)
   __pyx_builtin___import__ = __Pyx_GetBuiltinName(__pyx_n_s_import); if (!__pyx_builtin___import__) __PYX_ERR(1, 100, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 141, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 156, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 159, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(1, 373, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 408, __pyx_L1_error)
@@ -23862,16 +23950,16 @@
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
   /* "cfunc.to_py":67
- * @cname("__Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e")
- * cdef object __Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e((int, int)  (*f)(EditOperation) except *):
+ * @cname("__Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e")
+ * cdef object __Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e((int, int)  (*f)(EditOperation) except *):
  *     def wrap(EditOperation e):             # <<<<<<<<<<<<<<
  *         """wrap(e: 'EditOperation') -> '(int, int) '"""
  *         return f(e)
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_n_s_e); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
@@ -24147,14 +24235,15 @@
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_import_code(void); /*proto*/
 
 static int __Pyx_modinit_global_init_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_global_init_code", 0);
   /*--- Global init code ---*/
+  __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py = Py_None; Py_INCREF(Py_None);
   __pyx_collections_abc_Sequence = Py_None; Py_INCREF(Py_None);
   generic = Py_None; Py_INCREF(Py_None);
   strided = Py_None; Py_INCREF(Py_None);
   indirect = Py_None; Py_INCREF(Py_None);
   contiguous = Py_None; Py_INCREF(Py_None);
   indirect_contiguous = Py_None; Py_INCREF(Py_None);
   __Pyx_RefNannyFinishContext();
@@ -24184,15 +24273,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_t_1 = PyImport_ImportModule("prolothar_rule_mining.models.event_flow_graph.alignment.alignment_finder"); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder = __Pyx_ImportType_3_0_8(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.alignment.alignment_finder", "AlignmentFinder", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder = __Pyx_ImportType_3_0_10(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.alignment.alignment_finder", "AlignmentFinder", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_vtabptr_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration = &__pyx_vtable_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration;
   __pyx_vtable_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration._PathEnumeration__create_alignment = (struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment *(*)(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration *, PyObject *, PyObject *, __Pyx_memviewslice, int __pyx_skip_dispatch))__pyx_f_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_15PathEnumeration__PathEnumeration__create_alignment;
   #if CYTHON_USE_TYPE_SPECS
   __pyx_t_2 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16alignment_finder_AlignmentFinder); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration_spec, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -24220,30 +24309,30 @@
   if (__Pyx_MergeVtables(__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
   #endif
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_PathEnumeration, (PyObject *) __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_16path_enumeration_PathEnumeration) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_spec, NULL); if (unlikely(!__pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e)) __PYX_ERR(1, 66, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e_spec, __pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e) < 0) __PYX_ERR(1, 66, __pyx_L1_error)
+  __pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_spec, NULL); if (unlikely(!__pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e)) __PYX_ERR(1, 66, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e_spec, __pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e) < 0) __PYX_ERR(1, 66, __pyx_L1_error)
   #else
-  __pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e = &__pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e;
+  __pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e = &__pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e) < 0) __PYX_ERR(1, 66, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e) < 0) __PYX_ERR(1, 66, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
-  __pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e->tp_print = 0;
+  __pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e->tp_dictoffset && __pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e->tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_ptype___pyx_scope_struct____Pyx_CFunc___lParenint__comma_int__rParen__lParenEditOperation__rParen_to_py_1e->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e->tp_dictoffset && __pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype___pyx_scope_struct____Pyx_CFunc_3de20f__21prolothar_rule_mining_6models_16event_flow_g__etc_to_py_1e->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
   #if CYTHON_USE_TYPE_SPECS
   __pyx_array_type = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type___pyx_array_spec, NULL); if (unlikely(!__pyx_array_type)) __PYX_ERR(1, 114, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
@@ -24398,25 +24487,25 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("prolothar_common.levenshtein"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_16prolothar_common_11levenshtein_EditOperation = __Pyx_ImportType_3_0_8(__pyx_t_1, "prolothar_common.levenshtein", "EditOperation", sizeof(struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_16prolothar_common_11levenshtein_EditOperation) __PYX_ERR(2, 23, __pyx_L1_error)
+  __pyx_ptype_16prolothar_common_11levenshtein_EditOperation = __Pyx_ImportType_3_0_10(__pyx_t_1, "prolothar_common.levenshtein", "EditOperation", sizeof(struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_16prolothar_common_11levenshtein_EditOperation),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_16prolothar_common_11levenshtein_EditOperation) __PYX_ERR(2, 23, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("prolothar_rule_mining.models.event_flow_graph.node"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node = __Pyx_ImportType_3_0_8(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.node", "Node", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node = __Pyx_ImportType_3_0_10(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.node", "Node", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_4node_Node) __PYX_ERR(3, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("prolothar_rule_mining.models.event_flow_graph.alignment.alignment"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move = __Pyx_ImportType_3_0_8(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.alignment.alignment", "Move", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move) __PYX_ERR(4, 19, __pyx_L1_error)
+  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move = __Pyx_ImportType_3_0_10(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.alignment.alignment", "Move", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move) __PYX_ERR(4, 19, __pyx_L1_error)
   __pyx_vtabptr_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move = (struct __pyx_vtabstruct_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move*)__Pyx_GetVtable(__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move); if (unlikely(!__pyx_vtabptr_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Move)) __PYX_ERR(4, 19, __pyx_L1_error)
-  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment = __Pyx_ImportType_3_0_8(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.alignment.alignment", "Alignment", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment) __PYX_ERR(4, 27, __pyx_L1_error)
+  __pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment = __Pyx_ImportType_3_0_10(__pyx_t_1, "prolothar_rule_mining.models.event_flow_graph.alignment.alignment", "Alignment", sizeof(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment) __PYX_ERR(4, 27, __pyx_L1_error)
   __pyx_vtabptr_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment = (struct __pyx_vtabstruct_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment*)__Pyx_GetVtable(__pyx_ptype_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment); if (unlikely(!__pyx_vtabptr_21prolothar_rule_mining_6models_16event_flow_graph_9alignment_9alignment_Alignment)) __PYX_ERR(4, 27, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -24437,16 +24526,16 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("prolothar_common.levenshtein"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_3_0_8(__pyx_t_1, "compute_cost_matrix", (void (**)(void))&__pyx_f_16prolothar_common_11levenshtein_compute_cost_matrix, "__Pyx_memviewslice (PyObject *, PyObject *, struct __pyx_opt_args_16prolothar_common_11levenshtein_compute_cost_matrix *__pyx_optional_args)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_8(__pyx_t_1, "backtrace", (void (**)(void))&__pyx_f_16prolothar_common_11levenshtein_backtrace, "PyObject *(PyObject *, PyObject *, __Pyx_memviewslice, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "compute_cost_matrix", (void (**)(void))&__pyx_f_16prolothar_common_11levenshtein_compute_cost_matrix, "__Pyx_memviewslice (PyObject *, PyObject *, struct __pyx_opt_args_16prolothar_common_11levenshtein_compute_cost_matrix *__pyx_optional_args)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "backtrace", (void (**)(void))&__pyx_f_16prolothar_common_11levenshtein_backtrace, "PyObject *(PyObject *, PyObject *, __Pyx_memviewslice, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -24732,14 +24821,24 @@
   (void)__Pyx_modinit_variable_import_code();
   if (unlikely((__Pyx_modinit_function_import_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
+  /* "EnumTypeToPy":1
+ * cdef object __pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py = None             # <<<<<<<<<<<<<<
+ * 
+ * @cname("__Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py")
+ */
+  __Pyx_INCREF(Py_None);
+  __Pyx_XGOTREF(__pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py);
+  __Pyx_DECREF_SET(__pyx_imported_enum___Pyx_Enum_7e8028__16prolothar_common_11levenshtein_enum__dunderp__etc_to_py, Py_None);
+  __Pyx_GIVEREF(Py_None);
+
   /* "View.MemoryView":99
  * 
  * cdef object __pyx_collections_abc_Sequence "__pyx_collections_abc_Sequence"
  * try:             # <<<<<<<<<<<<<<
  *     if __import__("sys").version_info >= (3, 3):
  *         __pyx_collections_abc_Sequence = __import__("collections.abc").abc.Sequence
  */
@@ -27179,15 +27278,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -30071,18 +30170,18 @@
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_8
-#define __PYX_HAVE_RT_ImportType_3_0_8
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -30128,23 +30227,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_8 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_8 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -32953,17 +33052,17 @@
                        (int) (rt_version >> 24), (int) ((rt_version >> 16) & 0xFF)
        );
         return PyErr_WarnEx(NULL, message, 1);
     }
 }
 
 /* FunctionImport */
-  #ifndef __PYX_HAVE_RT_ImportFunction_3_0_8
-#define __PYX_HAVE_RT_ImportFunction_3_0_8
-static int __Pyx_ImportFunction_3_0_8(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportFunction_3_0_10
+#define __PYX_HAVE_RT_ImportFunction_3_0_10
+static int __Pyx_ImportFunction_3_0_10(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/path_enumeration.pyx` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/path_enumeration.pyx`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/petrinet.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/petrinet.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/alignment/sync_or_log_only.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/alignment/sync_or_log_only.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/caching.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/caching.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/cover/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/cover/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/cover/cover.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/cover/cover.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/cover/cover_computer.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/cover/cover_computer.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/cover/model_code_counter.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/cover/model_code_counter.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/edge.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/edge.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/graph.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/graph.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/node.cpp` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/node.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "language": "c++",
         "name": "prolothar_rule_mining.models.event_flow_graph.node",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -745,16 +775,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1098,15 +1133,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1185,15 +1220,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1284,32 +1319,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -9041,15 +9059,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/node.pyx` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/node.pyx`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/router/learning/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/router/learning/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/router/learning/oracle_router_learner.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/router/learning/oracle_router_learner.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/router/learning/rule_classifier_router_learner.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/router/learning/rule_classifier_router_learner.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/router/oracle_router.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/router/oracle_router.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/router/router.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/router/router.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/models/event_flow_graph/router/ruled_router.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/models/event_flow_graph/router/ruled_router.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/knn/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/knn/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/knn/knn.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/knn/knn.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/naive_bayes/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/naive_bayes/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/naive_bayes/categorical_naive_bayes.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/naive_bayes/categorical_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/naive_bayes/mixed_naive_bayes.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/naive_bayes/mixed_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/candidate.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/candidate.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/reliable_rule_miner.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/reliable_rule_miner.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/strategy/abstract.cpp` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/strategy/abstract.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "language": "c++",
         "name": "prolothar_rule_mining.rule_miner.classification.rce.strategy.abstract",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -745,16 +775,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1098,15 +1133,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1185,15 +1220,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1284,32 +1319,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -10654,24 +10672,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct___CandidateSearchStrategy__generate_equals_candidates *__pyx_freelist_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct___CandidateSearchStrategy__generate_equals_candidates[8];
 static int __pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct___CandidateSearchStrategy__generate_equals_candidates = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct___CandidateSearchStrategy__generate_equals_candidates(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct___CandidateSearchStrategy__generate_equals_candidates > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct___CandidateSearchStrategy__generate_equals_candidates)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct___CandidateSearchStrategy__generate_equals_candidates[--__pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct___CandidateSearchStrategy__generate_equals_candidates];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct___CandidateSearchStrategy__generate_equals_candidates));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -10696,15 +10716,15 @@
   Py_CLEAR(p->__pyx_v_class_label);
   Py_CLEAR(p->__pyx_v_class_label_vector_map);
   Py_CLEAR(p->__pyx_v_condition);
   Py_CLEAR(p->__pyx_v_dataset);
   Py_CLEAR(p->__pyx_v_effect);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct___CandidateSearchStrategy__generate_equals_candidates < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct___CandidateSearchStrategy__generate_equals_candidates)))) {
     __pyx_freelist_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct___CandidateSearchStrategy__generate_equals_candidates[__pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct___CandidateSearchStrategy__generate_equals_candidates++] = ((struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct___CandidateSearchStrategy__generate_equals_candidates *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -10837,24 +10857,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_1__CandidateSearchStrategy__generate_numeric_candidates *__pyx_freelist_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_1__CandidateSearchStrategy__generate_numeric_candidates[8];
 static int __pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_1__CandidateSearchStrategy__generate_numeric_candidates = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_1__CandidateSearchStrategy__generate_numeric_candidates(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_1__CandidateSearchStrategy__generate_numeric_candidates > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_1__CandidateSearchStrategy__generate_numeric_candidates)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_1__CandidateSearchStrategy__generate_numeric_candidates[--__pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_1__CandidateSearchStrategy__generate_numeric_candidates];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_1__CandidateSearchStrategy__generate_numeric_candidates));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -10880,15 +10902,15 @@
   Py_CLEAR(p->__pyx_v_class_label_vector_map);
   Py_CLEAR(p->__pyx_v_condition);
   Py_CLEAR(p->__pyx_v_condition_holds_vector);
   Py_CLEAR(p->__pyx_v_dataset);
   Py_CLEAR(p->__pyx_v_effect);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_1__CandidateSearchStrategy__generate_numeric_candidates < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_1__CandidateSearchStrategy__generate_numeric_candidates)))) {
     __pyx_freelist_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_1__CandidateSearchStrategy__generate_numeric_candidates[__pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_1__CandidateSearchStrategy__generate_numeric_candidates++] = ((struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_1__CandidateSearchStrategy__generate_numeric_candidates *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -11024,24 +11046,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_2__CandidateSearchStrategy__yield_condition_candidates *__pyx_freelist_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_2__CandidateSearchStrategy__yield_condition_candidates[8];
 static int __pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_2__CandidateSearchStrategy__yield_condition_candidates = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_2__CandidateSearchStrategy__yield_condition_candidates(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_2__CandidateSearchStrategy__yield_condition_candidates > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_2__CandidateSearchStrategy__yield_condition_candidates)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_2__CandidateSearchStrategy__yield_condition_candidates[--__pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_2__CandidateSearchStrategy__yield_condition_candidates];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_2__CandidateSearchStrategy__yield_condition_candidates));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -11068,15 +11092,15 @@
   Py_CLEAR(p->__pyx_v_b);
   Py_CLEAR(p->__pyx_v_interval);
   Py_CLEAR(p->__pyx_v_interval_list);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_7genexpr__pyx_v_v);
   Py_CLEAR(p->__pyx_v_value);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_2__CandidateSearchStrategy__yield_condition_candidates < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_2__CandidateSearchStrategy__yield_condition_candidates)))) {
     __pyx_freelist_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_2__CandidateSearchStrategy__yield_condition_candidates[__pyx_freecount_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_2__CandidateSearchStrategy__yield_condition_candidates++] = ((struct __pyx_obj_21prolothar_rule_mining_10rule_miner_14classification_3rce_8strategy_8abstract___pyx_scope_struct_2__CandidateSearchStrategy__yield_condition_candidates *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -16281,15 +16305,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/strategy/abstract.pyx` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/strategy/abstract.pyx`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/strategy/beam_search.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/strategy/beam_search.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rce/strategy/best_first.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rce/strategy/best_first.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/class_output_exception.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/class_output_exception.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/first_firing_rule_model.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/first_firing_rule_model.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/if_then_else_rule.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/if_then_else_rule.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/list_of_rules.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/list_of_rules.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/return_class_rule.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/return_class_rule.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/rule.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/rule.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/sklearn.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/sklearn.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/classification/rules/voting_class_rule.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/classification/rules/voting_class_rule.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/classification_miner.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/classification_miner.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/add_sequence_path_candidate.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/add_sequence_path_candidate.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/candidate.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/candidate.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/candidate_queue.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/candidate_queue.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/not_applicable_error.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/not_applicable_error.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/remove_chain_candidate.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/remove_chain_candidate.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/remove_edge_candidate.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/candidates/remove_edge_candidate.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/consequence.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/consequence.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/abstract.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/abstract.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/oracle.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/oracle.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/sequence_alignment_no_mdl.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/sequence_alignment_no_mdl.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/sequence_bottom_up.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/sequence_bottom_up.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/sequence_top_down.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/consequence/event_flow_graph_miner/sequence_top_down.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/adversarial_lstm.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/adversarial_lstm.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/base_lstm.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/base_lstm.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/batch_generator.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/batch_generator.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/callbacks.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/callbacks.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/plain_lstm.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/data_to_sequence_lstm/plain_lstm.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/dats.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/dats.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/event_classifier.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/event_classifier.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/append_rule.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/append_rule.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/append_subsequence.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/append_subsequence.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/blackbox.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/blackbox.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/classification_rule.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/classification_rule.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/event_flow_graph_rule.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/event_flow_graph_rule.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/export/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/export/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/export/html/error_highlighter.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/export/html/error_highlighter.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/if_then_else.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/if_then_else.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/list_of_rules.cpp` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/list_of_rules.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "language": "c++",
         "name": "prolothar_rule_mining.rule_miner.data_to_sequence.rules.list_of_rules",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -745,16 +775,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1098,15 +1133,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1185,15 +1220,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1284,32 +1319,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -12058,24 +12076,26 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct__yield_subrules *__pyx_freelist_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct__yield_subrules[8];
 static int __pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct__yield_subrules = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct__yield_subrules(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct__yield_subrules > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct__yield_subrules)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct__yield_subrules[--__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct__yield_subrules];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct__yield_subrules));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -12096,15 +12116,15 @@
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_rule);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct__yield_subrules < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct__yield_subrules)))) {
     __pyx_freelist_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct__yield_subrules[__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct__yield_subrules++] = ((struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct__yield_subrules *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -12225,24 +12245,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string *__pyx_freelist_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string[8];
 static int __pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string[--__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -12261,15 +12283,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_prefix);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string)))) {
     __pyx_freelist_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string[__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string++] = ((struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_1_to_string *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -12394,24 +12416,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_2_genexpr *__pyx_freelist_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_2_genexpr[8];
 static int __pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_2_genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_2_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_2_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_2_genexpr)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_2_genexpr[--__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_2_genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_2_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -12432,15 +12456,15 @@
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_outer_scope);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_rule);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_2_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_2_genexpr)))) {
     __pyx_freelist_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_2_genexpr[__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_2_genexpr++] = ((struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_2_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -12561,24 +12585,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_3_genexpr *__pyx_freelist_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_3_genexpr[8];
 static int __pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_3_genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_3_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_3_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_3_genexpr)))) {
     o = (PyObject*)__pyx_freelist_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_3_genexpr[--__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_3_genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_3_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -12598,15 +12624,15 @@
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_rule);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_3_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_3_genexpr)))) {
     __pyx_freelist_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_3_genexpr[__pyx_freecount_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_3_genexpr++] = ((struct __pyx_obj_21prolothar_rule_mining_10rule_miner_16data_to_sequence_5rules_13list_of_rules___pyx_scope_struct_3_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -19574,15 +19600,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/list_of_rules.pyx` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/list_of_rules.pyx`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/mdl.cpp` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/mdl.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "language": "c++",
         "name": "prolothar_rule_mining.rule_miner.data_to_sequence.rules.mdl",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -745,16 +775,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1098,15 +1133,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1185,15 +1220,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1284,32 +1319,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -12339,15 +12357,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/mdl.pyx` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/mdl.pyx`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/rule.cpp` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/rule.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "language": "c++",
         "name": "prolothar_rule_mining.rule_miner.data_to_sequence.rules.rule",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -745,16 +775,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1098,15 +1133,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1185,15 +1220,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1284,32 +1319,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -10371,15 +10389,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/rule.pyx` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/rule.pyx`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/rules/rule_literal.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/rules/rule_literal.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/window_classifier/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/window_classifier/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/window_classifier/window_classifier.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/window_classifier/window_classifier.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/data_to_sequence/window_classifier/window_rule.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/data_to_sequence/window_classifier/window_rule.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/dataset_splitting_miner.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/dataset_splitting_miner.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/multilabel/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/multilabel/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/multilabel/evaluation.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/multilabel/evaluation.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/multilabel/rules/output_fixed_set_rule.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/multilabel/rules/output_fixed_set_rule.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/multilabel/rules/rule.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/multilabel/rules/rule.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/deep_generator/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/deep_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/deep_generator/deep_generator.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/deep_generator/deep_generator.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/eventlog_iterator.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/eventlog_iterator.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/irons/irons.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/irons/irons.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/trivial/__init__.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/trivial/__init__.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/trivial/majority_event_predictor.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/trivial/majority_event_predictor.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining/rule_miner/next_event_prediction/trivial/prefix_aware_majority_predictor.py` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining/rule_miner/next_event_prediction/trivial/prefix_aware_majority_predictor.py`

 * *Files identical despite different names*

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining.egg-info/PKG-INFO` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: prolothar-rule-mining
-Version: 3.0.1
-Summary: algorithms for process mining and data mining on event sequences
-Home-page: https://gitlab.dillinger.de/KI/DataScience/processmining/prolothar-process-discovery
+Version: 3.0.2
+Summary: algorithms for prediction and rule mining on event sequences
+Home-page: https://github.com/shs-it/prolothar-rule-mining
 Author: Boris Wiegand
 Author-email: boris.wiegand@stahl-holding-saar.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyfim==6.28
@@ -105,16 +105,16 @@
 graph.plot()
 graph.plot(view=False, filepath='path_to_pdf')
 
 #get and print the classification rule at each node
 for node, router in rules_model.get_node_router_table().items():
     print('===============================')
     print(f'rule at node {node}')
-    print(node.get_rule())
-    # alternative: print(node.get_rule().to_html())
+    print(router.get_rule())
+    # alternative: print(router.get_rule().to_html())
 ```
 
 ## Development
 
 These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.
 
 ### Additional Prerequisites
@@ -130,16 +130,24 @@
 
 ```bash
 make test
 ```
 
 ### Deployment
 
+1. Change the version in version.txt
+2. Build and publish the package on pypi by
 ```bash
-make clean_package || make package && make publish
+make clean_package
+make package && make publish
+```
+3. Create and push a tag for this version by
+```bash
+git tag -a [version] -m "describe this version"
+git push --tags
 ```
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning.
 
 ## Authors
```

### Comparing `prolothar-rule-mining-3.0.1/prolothar_rule_mining.egg-info/SOURCES.txt` & `prolothar-rule-mining-3.0.2/prolothar_rule_mining.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,34 +24,39 @@
 prolothar_rule_mining/models/event_flow_graph/alignment/path_enumeration.cpp
 prolothar_rule_mining/rule_miner/classification/rce/strategy/abstract.cpp
 prolothar_rule_mining/rule_miner/data_to_sequence/rules/list_of_rules.cpp
 prolothar_rule_mining/rule_miner/data_to_sequence/rules/mdl.cpp
 prolothar_rule_mining/rule_miner/data_to_sequence/rules/rule.cpp
 prolothar_rule_mining/models/__init__.py
 prolothar_rule_mining/models/conditions.cpp
+prolothar_rule_mining/models/conditions.pxd
 prolothar_rule_mining/models/conditions.pyx
 prolothar_rule_mining/models/converter/eventflow_graph_to_pm4py_petrinet_converter.py
 prolothar_rule_mining/models/converter/sequence_to_class_dataset_converter.py
 prolothar_rule_mining/models/converter/sequence_to_multilabel_dataset_converter.py
 prolothar_rule_mining/models/dataset_generator/__init__.py
 prolothar_rule_mining/models/dataset_generator/classification.py
 prolothar_rule_mining/models/dataset_generator/data_to_sequence.py
 prolothar_rule_mining/models/dataset_generator/dataset_generator.py
+prolothar_rule_mining/models/event_flow_graph/__init__.pxd
 prolothar_rule_mining/models/event_flow_graph/__init__.py
 prolothar_rule_mining/models/event_flow_graph/caching.py
 prolothar_rule_mining/models/event_flow_graph/edge.py
 prolothar_rule_mining/models/event_flow_graph/graph.py
 prolothar_rule_mining/models/event_flow_graph/node.cpp
+prolothar_rule_mining/models/event_flow_graph/node.pxd
 prolothar_rule_mining/models/event_flow_graph/node.pyx
 prolothar_rule_mining/models/event_flow_graph/alignment/__init__.py
 prolothar_rule_mining/models/event_flow_graph/alignment/a_star.cpp
 prolothar_rule_mining/models/event_flow_graph/alignment/a_star.pyx
 prolothar_rule_mining/models/event_flow_graph/alignment/alignment.cpp
+prolothar_rule_mining/models/event_flow_graph/alignment/alignment.pxd
 prolothar_rule_mining/models/event_flow_graph/alignment/alignment.pyx
 prolothar_rule_mining/models/event_flow_graph/alignment/alignment_finder.cpp
+prolothar_rule_mining/models/event_flow_graph/alignment/alignment_finder.pxd
 prolothar_rule_mining/models/event_flow_graph/alignment/alignment_finder.pyx
 prolothar_rule_mining/models/event_flow_graph/alignment/beam_search.py
 prolothar_rule_mining/models/event_flow_graph/alignment/greedy_beam_search.py
 prolothar_rule_mining/models/event_flow_graph/alignment/greedy_shortest_path.py
 prolothar_rule_mining/models/event_flow_graph/alignment/heuristics.cpp
 prolothar_rule_mining/models/event_flow_graph/alignment/heuristics.pyx
 prolothar_rule_mining/models/event_flow_graph/alignment/partial_alignment.cpp
```

### Comparing `prolothar-rule-mining-3.0.1/setup.py` & `prolothar-rule-mining-3.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,26 +63,26 @@
 else:
     extensions = []
 
 # This call to setup() does all the work
 setup(
     name="prolothar-rule-mining",
     version=version,
-    description="algorithms for process mining and data mining on event sequences",
+    description="algorithms for prediction and rule mining on event sequences",
     long_description=README,
     long_description_content_type="text/markdown",
-    url="https://gitlab.dillinger.de/KI/DataScience/processmining/prolothar-process-discovery",
+    url="https://github.com/shs-it/prolothar-rule-mining",
     author="Boris Wiegand",
     author_email="boris.wiegand@stahl-holding-saar.de",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.11",
     ],
     packages=find_namespace_packages(
-        include=['prolothar_process_discovery*']
+        include=['prolothar_rule_mining*']
     ),
     include_package_data=True,
     package_data={
         "prolothar_rule_mining": [
             '*','*/*','*/*/*','*/*/*/*','*/*/*/*/*',
             '*/*/*/*/*/*','*/*/*/*/*/*/*','*/*/*/*/*/*/*/*'
         ]
```

